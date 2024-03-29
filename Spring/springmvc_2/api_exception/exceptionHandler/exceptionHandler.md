# API 예외 처리 - @ExceptionHandler

- ErrorResult
```java
@Data
@AllArgsConstructor
public class ErrorResult {
    private String code;
    private String message;
}
```

- 컨트롤러
```java
@RestController
@Slf4j
public class ApiExceptionV2Controller {

    @ResponseStatus(HttpStatus.BAD_REQUEST)
    @ExceptionHandler(IllegalArgumentException.class)
    public ErrorResult illegalExHandler(IllegalArgumentException e) {
        log.error("[exceptionHandler] ex", e);
        return new ErrorResult("BAD", e.getMessage());
    }
    
    @ExceptionHandler
    public ResponseEntity<ErrorResult> userExHandler(UserException e) {
        log.error("[exceptionHandler] ex", e);
        ErrorResult errorResult = new ErrorResult("USER-EX", e.getMessage());
        return new ResponseEntity<>(errorResult, HttpStatus.BAD_REQUEST);
    }

    @ResponseStatus(HttpStatus.INTERNAL_SERVER_ERROR)
    @ExceptionHandler
    public ErrorResult exHandler(Exception e) {
        log.error("[exceptionHandler] ex", e);
        return new ErrorResult("EX", "내부 오류");
    }

    @GetMapping("/api2/members/{id}")
    public MemberDto getMember(@PathVariable("id") String id) {

        if (id.equals("ex")) {
            throw new RuntimeException("잘못된 사용자");
        }

        if (id.equals("bad")) {
            throw new IllegalArgumentException("잘못된 입력 값");
        }

        if (id.equals("user-ex")) {
            throw new UserException("사용자 오류");
        }

        return new MemberDto(id, "hello " + id);
    }

    @Data
    @AllArgsConstructor
    static class MemberDto {
        private String memberId;
        private String name;
    }
}
```
`@ExceptionHandler` 어노테이션을 선언하고 해당 컨트롤러에서 처리하고 싶은 예외를 지정한다. 해당 컨트롤러에서 예외가 발생하면 이 메서드가 호출된다.
지정한 예외 또는 그 예외의 자식 클래스는 모두 잡을 수 있다. 당연히 항상 자세한 것이 우선권을 가진다.

다양한 예외를 한 번에 처리할 수도 있다.
```java
@ExceptionHandler({AException.class, BException.class}) 
public String ex(Exception e) {
    log.info("exception e", e); 
}
```
`@ExceptionHandler`에 예외를 생략하면 메서드 파라미터의 예외가 지정된다.(`UserException`같은 경우)

`@ExceptionHandler`는 다양한 파라미터와 응답을 지정할 수 있다. [공식 매뉴얼](https://docs.spring.io/spring-framework/reference/web/webmvc/mvc-controller/ann-exceptionhandler.html#mvc-ann-exceptionhandler-args)

예를 들어 `/api2/members/bad`를 호출 했을 때 실행 흐름
- 컨트롤러를 호출한 결과 `IllegalArgumentException` 예외가 컨트롤러 밖으로 던져진다.
- 예외가 발생했으므로 `ExceptionResovler`가 작동한다. 이 때 가장 우선순위가 높은 `ExceptionHandlerExceptionResolver`가 실행된다.
- `ExceptionHandlerExceptionResolver`는 해당 컨트롤러에 `IllegalArgumentException`를 처리할 수 있는 `@ExceptionHandler`가 있는지 확인한다.
- `illegalExHandler()`를 실행한다. `@RestController`이므로 HTTP 컨버터가 사용돼 응답이 JSON으로 반환된다.
  - `@ResponseStatsu`를 지정했으므로 HTTP 상태 코드 400으로 응답한다.

`RuntimeException`은 `Exception`의 자식 클래스 이기 때문에 `exHandler` 메서드가 호출된다.

## @ControllerAdvice
> `@ExceptionHandler`로 예외를 깔끔하게 처리할 수 있지만 정상 코드와 예외 처리 코드가 하나의 컨트롤러에 섞여 있다. `@ControllerAdvice`로 분리할 수 있다.
- ControllerAdvice
```java
@Slf4j
@RestControllerAdvice
public class ExControllerAdvice {

    @ResponseStatus(HttpStatus.BAD_REQUEST)
    @ExceptionHandler(IllegalArgumentException.class)
    public ErrorResult illegalExHandler(IllegalArgumentException e) {
        log.error("[exceptionHandler] ex", e);
        return new ErrorResult("BAD", e.getMessage());
    }

    @ExceptionHandler
    public ResponseEntity<ErrorResult> userExHandler(UserException e) {
        log.error("[exceptionHandler] ex", e);
        ErrorResult errorResult = new ErrorResult("USER-EX", e.getMessage());
        return new ResponseEntity<>(errorResult, HttpStatus.BAD_REQUEST);
    }

    @ResponseStatus(HttpStatus.INTERNAL_SERVER_ERROR)
    @ExceptionHandler
    public ErrorResult exHandler(Exception e) {
        log.error("[exceptionHandler] ex", e);
        return new ErrorResult("EX", "내부 오류");
    }
}
```
- 컨트롤러
```java
@RestController
@Slf4j
public class ApiExceptionV2Controller {

    @GetMapping("/api2/members/{id}")
    public MemberDto getMember(@PathVariable("id") String id) {

        if (id.equals("ex")) {
            throw new RuntimeException("잘못된 사용자");
        }

        if (id.equals("bad")) {
            throw new IllegalArgumentException("잘못된 입력 값");
        }

        if (id.equals("user-ex")) {
            throw new UserException("사용자 오류");
        }

        return new MemberDto(id, "hello " + id);
    }

    @Data
    @AllArgsConstructor
    static class MemberDto {
        private String memberId;
        private String name;
    }
}
```
- `@ControllerAdivce`는 대상으로 지정한 여러 컨트롤러에 `@ExceptionHandler`, `@InitBinder` 기능을 부여해주는 역할을 한다.
- 대상 컨트롤러 지정 방법
```java
// Target all Controllers annotated with @RestController
@ControllerAdvice(annotations = RestController.class)
public class ExampleAdvice1 {}

// Target all Controllers within specific packages
@ControllerAdvice("org.example.controllers")
public class ExampleAdvice2 {}

// Target all Controllers assignable to specific classes
@ControllerAdvice(assignableTypes = {ControllerInterface.class, AbstractController.class})
public class ExampleAdvice3 {}
```
- 특정 어노테이션이 있는 컨트롤러 지정, 특정 패키지를 직접 지정(해당 패키지와 그 하위에 있는 컨트롤러가 대상이 된다.), 특정 클래스를 지정할 수도 있다.
  - 대상 컨트롤러 지정을 생략하면 모든 컨트롤러에 글로벌 하게 적용된다.