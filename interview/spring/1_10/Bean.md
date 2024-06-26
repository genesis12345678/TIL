# 스프링 컨테이너와 스프링 빈에 대해 설명해 주세요.

## 스프링 컨테이너
- 스프링 컨테이너는 자바 객체의 생명 주기를 관리하는 공간을 말한다.
- 스프링에서는 자바 객체를 **스프링 빈(`Bean`)** 이라고 하고, 스프링 컨테이너에는 [IoC/DI](https://www.acmicpc.net/problem/2211) 원리가 적용된다.
- 스프링 컨테이너의 DI 없이 개발자가 직접 의존성을 주입하고 관리하려면, 그 객체가 어떤 객체를 필요로 하는지 일일이 확인하면서 주입해야 하기에 쉽지 않은 작업일 것이다.
- 대신 스프링 컨테이너가 객체의 생성부터 소멸까지 생명주기부터 의존성 주입을 대신 해주기 때문에 제어의 흐름을 외부에 맡길 수 있게 되는 것이다.(`IoC`)
- 스프링 컨테이너가 의존성을 주입해주는 방법(`DI`)
  - **생성자 주입**(`@RequiredArgsConstructor`)
  - 수정자 주입(`setter`)
  - 필드 주입(`@Autowired`)
  - `init`같은 일반 메서드 주입
- 스프링은 불변으로 안전하게 설계할 수 있는 **생성자 주입**을 권장한다.

**스프링 컨테이너는 스프링 빈을 싱글톤으로 관리하기 때문에 다음과 같은 주의사항이 있다.**
- 여러 클라이언트가 같은 인스턴스를 공유하기 때문에 상태를 유지하게 설계하면 안 된다.
- 공유 필드에 주의해야 한다.

**스프링 컨테이너가 스프링 빈을 관리해주기 때문에 다음과 같은 이점이 생긴다.**
- 개발자는 복잡한 의존성을 주입하는 과정에 신경쓰지 않고 의존성을 사용하는 로직에만 집중할 수 있다.
- 의존성이 주입 될 객체가 항상 싱글 오브젝트임을 보장해준다.

**스프링 컨테이너가 의존성을 주입하기 위해 조회한 빈이 2개 이상이면?**
- `@Bean`을 이용해 수동으로 빈 등록을 할 수 있다.
- `@Autowired`로 필드 주입 시에는 필드명을 원하는 클래스가 스프링 빈으로 등록되도록 변경할 수 있다.
- `@Quailfier`로 이름을 부여해 의존성이 필요한 곳에서 `@Quailfier`를 붙여 이름을 적어줄 수 있다.
- `@Primary`로 우선순위를 지정할 수 있다.

## 스프링 빈

- **스프링 빈은 인스턴스화된 객체를 의미하며, 스프링 컨테이너에 등록돼 스프링 컨테이너가 관리하는 객체를 스프링 빈이라고 한다.**
- 개발자는 `@Bean`이나 `@ComponentScan`의 대상이 되는 애노테이션을 사용해 필요한 클래스를 스프링 컨테이너에 빈으로 등록할 수 있다.

스프링 빈은 다음과 같은 생명주기를 가진다.

![img_1.png](image/img_1.png)

- **초기화 콜백** : 빈이 생성되고 빈의 의존관계 주입이 완료된 후 호출
- **소멸전 콜백** : 빈이 소멸되기 직전에 호출

**스프링은 빈 생명주기 콜백을 관리하는 여러가지 기능들을 제공한다.**
- **인터페이스**
  - `InitializingBean`,`DisposableBean` 인터페이스의 각각 `afterPropertiesSet()`, `destroy()` 메서드로 초기화와 소멸을 지원한다.
  - 스프링 전용 인터페이스이다.
- **메서드 지정**
  - `@Bean`의 `initMethod`, `destroyMethod` 속성으로 초기화, 소멸 메서드를 지정할 수 있다.
- **어노테이션**
  - `@PostConstruct`, `@PreDestroy`로 메서드에 선언해 초기화, 소멸 메서드임을 명시할 수 있다.
  - 가장 간편한 방법이며, 스프링이 아닌 자바 표준 기술이다.

**스프링은 싱글톤 외에 다양한 빈 스코프를 지원한다.**
- **싱글톤** : 기본 스코프로, 스프링 컨테이너의 시작과 종료까지 유지되는 가장 넓은 범위의 스코프다.
- **프로토타입** : 항상 새로운 인스턴스를 생성해서 반환하는 스코프다.
  - 의존관계 주입까지만 관여하고 더는 관리하지 않는 매우 짧은 범위의 스코프다.
- **웹 스코프** : 웹 환경에서만 동작하는 스코프로, 종료시점까지 관리한다.
  - 종류로는 `request`, `session`, `application`, `websocket`이 있다.

<br>

### 참고
- [참고 블로그](https://ittrue.tistory.com/221)
- [참고 동영상](https://www.youtube.com/watch?v=3gURJvJw_T4)