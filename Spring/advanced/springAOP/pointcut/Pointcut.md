# 스프링 AOP - 포인트컷

## 포인트컷 지시자

- 포인트컷 지시자의 종류
  - `execution` : 메서드 실행 조인 포인트를 매칭한다. 스프링 AOP에서 가장 많이 사용하고 기능도 복잡하다.
  - `within` : 특정 타입 내의 조인 포인트를 매칭한다.
  - `args` : 인자가 주어진 타입의 인스턴스인 조인 포인트
  - `this` : 스프링 빈 객체(스프링 AOP 프록시)를 대상으로 하는 조인 포인트
  - `target` : Target 객체(스프링 AOP가 가리키는 실제 대상)를 대상으로 하는 조인 포인트
  - `@target` : 실행 객체의 클래스에 주어진 타입의 어노테이션이 있는 조인 포인트
  - `@within` : 주어진 어노테이션이 있는 타입 내 조인 포인트
  - `@annotation` : 메서드가 주어진 어노테이션을 가지고 있는 조인 포인트를 매칭
  - `@args` : 전달된 실제 인수의 런타입 타입이 주어진 타입의 어노테이션을 갖는 조인 포인트
  - `bean` : 스프링 전용 포인트컷 지시자로, 빈의 이름으로 포인트컷을 지정한다.

`execution`을 가장 많이 사용하고 나머지는 자주 사용하지 않는다.

## 예제
```java
@Target(ElementType.TYPE)
@Retention(RetentionPolicy.RUNTIME)
public @interface ClassAop {
}

@Target(ElementType.METHOD)
@Retention(RetentionPolicy.RUNTIME)
public @interface MethodAop {
    String value();
}
```
```java
public interface MemberService {
    String hello(String param);
}

@ClassAop
@Component
public class MemberServiceImpl implements MemberService{

    @Override
    @MethodAop("test value")
    public String hello(String param) {
        return "ok";
    }

    public String internal(String param) {
        return "ok";
    }
}
```
```java
@Slf4j
public class ExecutionTest {

    AspectJExpressionPointcut pointcut = new AspectJExpressionPointcut();
    Method helloMethod;

    @BeforeEach
    public void init() throws NoSuchMethodException {
        helloMethod = MemberServiceImpl.class.getMethod("hello", String.class);
    }

    @Test
    void printMethod() {
        //public java.lang.String hello.aop.member.MemberServiceImpl.hello(java.lang.String)
        log.info("helloMethod={}", helloMethod);
    }
}
```
- `AspectJExpressionPointcut`은 포인트컷 표현식을 처리해주는 클래스다. 여기에 포인트컷 표현식을 지정하면 된다.
- `AspectJExpressionPointcut` 상위에 `Pointcut` 인터페이스가 있다.
- `printMethod()`에서 나온 출력값으로 `execution`을 사용할 수 있다.

<br>

- [execution](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/springAOP/pointcut/Pointcut_1.md#execution)
- [within](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/springAOP/pointcut/Pointcut_2.md#within)
- [args](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/springAOP/pointcut/Pointcut_2.md#args)
- [@target, @within](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/springAOP/pointcut/Pointcut_2.md#target-within)
- [@annotation](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/springAOP/pointcut/Pointcut_3.md#annotation)
- [bean](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/springAOP/pointcut/Pointcut_3.md#bean)
- [매개변수 전달](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/springAOP/pointcut/Pointcut_3.md#%EB%A7%A4%EA%B0%9C%EB%B3%80%EC%88%98-%EC%A0%84%EB%8B%AC)
- [this, target](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/springAOP/pointcut/Pointcut_3.md#this%EC%99%80-target)