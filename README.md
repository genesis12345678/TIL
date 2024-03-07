# TIL 📃

## INDEX 🔍

### Spring

<details>
    <summary>스프링 핵심 원리</summary>

<details>
    <summary>기본</summary>

- [메인](https://github.com/genesis12345678/TIL/blob/main/Spring/basic/spring_basic.md#%EC%8A%A4%ED%94%84%EB%A7%81-%ED%95%B5%EC%8B%AC-%EA%B8%B0%EB%B3%B8-%EC%9B%90%EB%A6%AC)
- [순수 자바 설계(1)](https://github.com/genesis12345678/TIL/blob/main/Spring/basic/pureJava/java_1.md#%EC%88%9C%EC%88%98%ED%95%9C-%EC%9E%90%EB%B0%94%EB%A7%8C%EC%9C%BC%EB%A1%9C-%EC%84%A4%EA%B3%84---1) - 스프링 기술 없이 자바만으로 설계할 때 문제점
- [순수 자바 설계(2)](https://github.com/genesis12345678/TIL/blob/main/Spring/basic/pureJava/java_2.md#%EC%88%9C%EC%88%98%ED%95%9C-%EC%9E%90%EB%B0%94%EB%A7%8C%EC%9C%BC%EB%A1%9C-%EC%84%A4%EA%B3%84---2) - 자바만으로 설계했을 때 문제점을 해결해보고 스프링 기술 접목해보기
- [스프링 컨테이너(1)](https://github.com/genesis12345678/TIL/blob/main/Spring/basic/springContainer/container_1.md#%EC%8A%A4%ED%94%84%EB%A7%81-%EC%BB%A8%ED%85%8C%EC%9D%B4%EB%84%88---1) - 스프링 컨테이너 생성 과정과 컨테이너에 등록된 빈 조회하는 법
- [스프링 컨테이너(2)](https://github.com/genesis12345678/TIL/blob/main/Spring/basic/springContainer/container_2.md#%EC%8A%A4%ED%94%84%EB%A7%81-%EC%BB%A8%ED%85%8C%EC%9D%B4%EB%84%88---2) - 스프링 빈을 생성하는 여러가지 방법(`BeanFactory`와 `ApplicationContext`)
- [싱글톤 컨테이너(1)](https://github.com/genesis12345678/TIL/blob/main/Spring/basic/singleton/singleton_1.md#%EC%8B%B1%EA%B8%80%ED%86%A4-%EC%BB%A8%ED%85%8C%EC%9D%B4%EB%84%88---1) - 싱글톤 패턴과 싱글톤 방식의 주의점(공유필드)
- [싱글톤 컨테이너(2)](https://github.com/genesis12345678/TIL/blob/main/Spring/basic/singleton/singleton_2.md#%EC%8B%B1%EA%B8%80%ED%86%A4-%EC%BB%A8%ED%85%8C%EC%9D%B4%EB%84%88---2) - `@Configuration`에 대해
- [컴포넌트 스캔](https://github.com/genesis12345678/TIL/blob/main/Spring/basic/componentScan/componentScan.md#%EC%8A%A4%ED%94%84%EB%A7%81-%EC%BB%B4%ED%8F%AC%EB%84%8C%ED%8A%B8-%EC%8A%A4%EC%BA%94) - 자동 빈 등록
- [의존관계 자동 주입(1)](https://github.com/genesis12345678/TIL/blob/main/Spring/basic/DI/DI_1.md#%EC%8A%A4%ED%94%84%EB%A7%81-%EC%9D%98%EC%A1%B4%EA%B4%80%EA%B3%84-%EC%9E%90%EB%8F%99-%EC%A3%BC%EC%9E%85---1) - 다양한 의존관계 주입 방법
- [의존관계 자동 주입(2)](https://github.com/genesis12345678/TIL/blob/main/Spring/basic/DI/DI_2.md#%EC%8A%A4%ED%94%84%EB%A7%81-%EC%9D%98%EC%A1%B4%EA%B4%80%EA%B3%84-%EC%9E%90%EB%8F%99-%EC%A3%BC%EC%9E%85---2) - 조회한 빈이 2개 이상일 때 구분하는 방법
- [빈 생명주기](https://github.com/genesis12345678/TIL/blob/main/Spring/basic/beanLifeCycle/beanLifeCycle.md#%EB%B9%88-%EC%83%9D%EB%AA%85%EC%A3%BC%EA%B8%B0-%EC%BD%9C%EB%B0%B1) - 스프링 빈의 생명주기 관리
- [빈 스코프(1)](https://github.com/genesis12345678/TIL/blob/main/Spring/basic/beanScope/beanScope_1.md#%EC%8A%A4%ED%94%84%EB%A7%81-%EB%B9%88-%EC%8A%A4%EC%BD%94%ED%94%84---1) - 스프링의 다양한 빈 스코프, 프로토타입 스코프
- [빈 스코프(2)](https://github.com/genesis12345678/TIL/blob/main/Spring/basic/beanScope/beanScope_2.md#%EC%8A%A4%ED%94%84%EB%A7%81-%EB%B9%88-%EC%8A%A4%EC%BD%94%ED%94%84---2) - 스프링이 다양한 빈 스코프, 웹 스코프

</details>

<details>
    <summary>고급</summary>

- [메인](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/LogTrace.md#%EB%A1%9C%EA%B7%B8-%EC%B6%94%EC%A0%81%EA%B8%B0)
- 로그 추적기 개발
  - [V1](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/logTrace_1/LogTrace_1.md#%EB%A1%9C%EA%B7%B8-%EC%B6%94%EC%A0%81%EA%B8%B0---v1) - 가장 원초적인 방법
  - [V2](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/logTrace_2/LogTrace_2.md#%EB%A1%9C%EA%B7%B8-%EC%B6%94%EC%A0%81%EA%B8%B0---v2) - 동기화 문제 발생
  - [V3](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/logTrace_3/LogTrace_3.md#%EB%A1%9C%EA%B7%B8-%EC%B6%94%EC%A0%81%EA%B8%B0---v3) - 필드 동기화 사용, 동시성 문제 발생
  - [V4](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/logTrace_4/LogTrace_4.md#%EB%A1%9C%EA%B7%B8-%EC%B6%94%EC%A0%81%EA%B8%B0---v4) - 템플릿 메서드 패턴 적용
  - [V5](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/logTrace_5/LogTrace_5.md#%EB%A1%9C%EA%B7%B8-%EC%B6%94%EC%A0%81%EA%B8%B0---v5) - 템플릿 콜백 패턴 적용
- [동시성 문제](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/syncProblem/SyncProblem.md#%EB%8F%99%EC%8B%9C%EC%84%B1-%EB%AC%B8%EC%A0%9C---%EC%98%88%EC%A0%9C) - 동시성 문제에 대해
- [쓰레드 로컬](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/threadLocal/ThreadLocal.md#%EC%93%B0%EB%A0%88%EB%93%9C-%EB%A1%9C%EC%BB%AC) - 동시성 문제를 해결하는 쓰레드 로컬에 대해
- [템플릿 메서드 패턴](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/templateMethodPattern/TemplateMethodPattern.md#%ED%85%9C%ED%94%8C%EB%A6%BF-%EB%A9%94%EC%84%9C%EB%93%9C-%ED%8C%A8%ED%84%B4) - 템플릿 메서드 패턴에 대해
- [전략 패턴](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/strategyPattern/StrategyPattern.md#%EC%A0%84%EB%9E%B5-%ED%8C%A8%ED%84%B4) - 전략 패턴에 대해
- [프록시 적용](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/proxyAndDecorator/Proxy.md) - 인터페이스 기반 프록시와 구체 클래스 기반 프록시
  - [프록시 패턴](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/proxyAndDecorator/proxy/Proxy.md#%ED%94%84%EB%A1%9D%EC%8B%9C-%ED%8C%A8%ED%84%B4) - 프록시 패턴에 대해
  - [데코레이터 패턴](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/proxyAndDecorator/proxy/Proxy.md#%EB%8D%B0%EC%BD%94%EB%A0%88%EC%9D%B4%ED%84%B0-%ED%8C%A8%ED%84%B4) - 데코레이터 패턴에 대해
- [JDK 동적 프록시](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/jdkDynamicProxy/JDKDynamicProxy.md#jdk-%EB%8F%99%EC%A0%81-%ED%94%84%EB%A1%9D%EC%8B%9C) - JDK 동적 프록시에 대해
  - [JDK 동적 프록시 적용](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/jdkDynamicProxy/JDKDynamicProxy.md#jdk-%EB%8F%99%EC%A0%81-%ED%94%84%EB%A1%9D%EC%8B%9C-%EC%A0%81%EC%9A%A9)
- [CGLIB](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/cglib/CGLIB.md#cglib) - `CGLIB`과 프록시 팩토리에 대해
  - [프록시 팩토리 적용](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/cglib/ApplyProxyFactory.md#%ED%94%84%EB%A1%9D%EC%8B%9C-%ED%8C%A9%ED%86%A0%EB%A6%AC-%EC%A0%81%EC%9A%A9)
- [포인트컷, 어드바이스, 어드바이저](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/advisor/Advisor.md#%ED%8F%AC%EC%9D%B8%ED%8A%B8%EC%BB%B7-%EC%96%B4%EB%93%9C%EB%B0%94%EC%9D%B4%EC%8A%A4-%EC%96%B4%EB%93%9C%EB%B0%94%EC%9D%B4%EC%A0%80) - 포인트컷, 어드바이스, 어드바이저에 대해
- [빈 후처리기](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/beanPostProcessor/BeanPostProcessor.md#%EB%B9%88-%ED%9B%84%EC%B2%98%EB%A6%AC%EA%B8%B0) - 프록시 팩토리를 적용했을 때 문제점을 해결하는 빈 후처리기에 대해
  - [빈 후처리기 적용](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/beanPostProcessor/BeanPostProcessor.md#%EC%95%A0%ED%94%8C%EB%A6%AC%EC%BC%80%EC%9D%B4%EC%85%98-%EB%B9%88-%ED%9B%84%EC%B2%98%EB%A6%AC%EA%B8%B0-%EC%A0%81%EC%9A%A9)
  - [스프링이 제공하는 빈 후처리기](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/beanPostProcessor/SpringBeanPostProcessor.md#%EC%8A%A4%ED%94%84%EB%A7%81%EC%9D%B4-%EC%A0%9C%EA%B3%B5%ED%95%98%EB%8A%94-%EB%B9%88-%ED%9B%84%EC%B2%98%EB%A6%AC%EA%B8%B0) - 스프링 AOP 기술 접목
- [@Aspect AOP](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/aspectAOP/AspectProxy.md#aspect-aop) - `@Aspect`에 대해
- 스프링 AOP
  - [개념](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/springAOP/idea/SpringAopIdea.md#%EC%8A%A4%ED%94%84%EB%A7%81-aop-%EA%B0%9C%EB%85%90) - 스프링 AOP에 대해 개념적으로 이해하기(적용 방식, 용어 등)
  - [구현](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/springAOP/implement/SpringAopImplement.md#%EC%8A%A4%ED%94%84%EB%A7%81-aop-%EA%B5%AC%ED%98%84%ED%95%98%EA%B8%B0) - 스프링 AOP 구현
    - [V1](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/springAOP/implement/SpringAopImplement_1_3.md#%EC%8A%A4%ED%94%84%EB%A7%81-aop-%EA%B5%AC%ED%98%84---v1) - `@Aspect` 사용
    - [V2](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/springAOP/implement/SpringAopImplement_1_3.md#%EC%8A%A4%ED%94%84%EB%A7%81-aop-%EA%B5%AC%ED%98%84---v2) - 포인트컷 분리해보기
    - [V3](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/springAOP/implement/SpringAopImplement_1_3.md#%EC%8A%A4%ED%94%84%EB%A7%81-aop-%EA%B5%AC%ED%98%84---v3) - 어드바이스 여러 개 적용
    - [V4](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/springAOP/implement/SpringAopImplement_4_6.md#%EC%8A%A4%ED%94%84%EB%A7%81-aop-%EA%B5%AC%ED%98%84---v4) - 포인트컷을 외부 클래스로 분리
    - [V5](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/springAOP/implement/SpringAopImplement_4_6.md#%EC%8A%A4%ED%94%84%EB%A7%81-aop-%EA%B5%AC%ED%98%84---v5) - 어드바이스 순서 지정
    - [V6](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/springAOP/implement/SpringAopImplement_4_6.md#%EC%8A%A4%ED%94%84%EB%A7%81-aop-%EA%B5%AC%ED%98%84---v6) - 어드바이스 종류에 대해
  - [포인트컷](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/springAOP/pointcut/Pointcut.md#%EC%8A%A4%ED%94%84%EB%A7%81-aop---%ED%8F%AC%EC%9D%B8%ED%8A%B8%EC%BB%B7) - 여러 포인트컷 지시자에 대해
    - [execution](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/springAOP/pointcut/Pointcut_1.md#%ED%8F%AC%EC%9D%B8%ED%8A%B8%EC%BB%B7-%EC%A7%80%EC%8B%9C%EC%9E%90) - `execution` 문법
    - [within](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/springAOP/pointcut/Pointcut_2.md#within) - `within` 문법
    - [args](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/springAOP/pointcut/Pointcut_2.md#args) - `args` 문법
    - [@target, @within](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/springAOP/pointcut/Pointcut_2.md#target-within) - `@target`, `@within`에 대해
    - [@annotation](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/springAOP/pointcut/Pointcut_3.md#annotation) - `@annotation`에 대해
    - [bean](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/springAOP/pointcut/Pointcut_3.md#bean) - `bean`에 대해
    - [매개변수 전달](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/springAOP/pointcut/Pointcut_3.md#%EB%A7%A4%EA%B0%9C%EB%B3%80%EC%88%98-%EC%A0%84%EB%8B%AC) - 포인트컷 표현식을 사용하여 어드바이스에 매개변수 전달
    - [this, target](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/springAOP/pointcut/Pointcut_3.md#this%EC%99%80-target) - `this`와 `target`에 대해
  - [예제]() - 스프링 AOP를 활용하여 로그 출력과 재시도를 하는 AOP 구현해보기
  - 주의사항 - 스프링 AOP 주의사항
    - [프록시 내부 호출](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/springAOP/warn/Warn_1.md#%EC%8A%A4%ED%94%84%EB%A7%81-aop-%EC%A3%BC%EC%9D%98%EC%82%AC%ED%95%AD) - 프록시 내부 호출 문제와 여러가지 대안
    - [프록시 기술과 한계](https://github.com/genesis12345678/TIL/blob/main/Spring/advanced/springAOP/warn/Warn_2.md#%EC%8A%A4%ED%94%84%EB%A7%81-aop-%EC%A3%BC%EC%9D%98%EC%82%AC%ED%95%AD) - 프록시 기술의 한계(타입 캐스팅, 의존관계 주입, CGLIB)와 스프링의 해결책
</details>
</details>

<details>
    <summary>스프링 MVC</summary>
<details>
    <summary>1편</summary>

- [메인](https://github.com/genesis12345678/TIL/blob/main/Spring/springmvc_1/springmvc_1.md#spring-mvc---1)
- [웹 애플리케이션](https://github.com/genesis12345678/TIL/blob/main/Spring/springmvc_1/web_application/web_application.md#web-application) - 웹 애플리케이션에 대한 전반적인 이해
- [서블릿](https://github.com/genesis12345678/TIL/blob/main/Spring/springmvc_1/servlet/servlet.md#%EC%84%9C%EB%B8%94%EB%A6%BF) - 서블릿 컨테이너 동작 방식과 `HttpServletRequest`, `HttpServletResponse`에 대해
- [JSP, MVC 패턴](https://github.com/genesis12345678/TIL/blob/main/Spring/springmvc_1/jsp_mvc/jsp_mvc.md#jsp%EC%99%80-mvc-%ED%8C%A8%ED%84%B4) - 서블릿과 JSP, MVC 패턴에 대해
- [MVC 프레임워크 만들기](https://github.com/genesis12345678/TIL/blob/main/Spring/springmvc_1/make_mvc/mvc.md#%ED%94%84%EB%A1%A0%ED%8A%B8-%EC%BB%A8%ED%8A%B8%EB%A1%A4%EB%9F%AC-%ED%8C%A8%ED%84%B4) - 프론트 컨트롤러 패턴으로 직접 MVC 프레임워크를 만들어보면서 컨트롤러에 대해 이해하기
- [스프링 MVC 구조](https://github.com/genesis12345678/TIL/blob/main/Spring/springmvc_1/spring_mvc/spring_mvc.md#%EC%8A%A4%ED%94%84%EB%A7%81-mvc-%EA%B5%AC%EC%A1%B0) - MVC 프레임워크를 직접 만들어 본 것을 기반으로 스프링 MVC 구조 이해하기
- [스프링 MVC 기본 기능](https://github.com/genesis12345678/TIL/blob/main/Spring/springmvc_1/springmvc_feature/feature.md#%EC%8A%A4%ED%94%84%EB%A7%81-mvc---%EA%B8%B0%EB%B3%B8-%EA%B8%B0%EB%8A%A5) - 스프링 MVC가 지원하는 요청과 응답의 여러가지 기능
</details>

<details>
    <summary>2편</summary>

- [메인](https://github.com/genesis12345678/TIL/blob/main/Spring/springmvc_2/springmvc_2.md#spring-mvc---2)
- [타임리프 기본 기능](https://github.com/genesis12345678/TIL/blob/main/Spring/springmvc_2/thymeleaf/thymeleaf.md#%ED%83%80%EC%9E%84%EB%A6%AC%ED%94%84) - 타임리프와 타임리프 기본 문법
- [타임리프와 스프링](https://github.com/genesis12345678/TIL/blob/main/Spring/springmvc_2/thymeleaf_spring/thymeleaf_spring.md#%ED%83%80%EC%9E%84%EB%A6%AC%ED%94%84---%EC%8A%A4%ED%94%84%EB%A7%81-%ED%86%B5%ED%95%A9) - 타임리프와 스프링 통합
- [메시지, 국제화](https://github.com/genesis12345678/TIL/blob/main/Spring/springmvc_2/message/message.md#%EB%A9%94%EC%8B%9C%EC%A7%80-%EA%B5%AD%EC%A0%9C%ED%99%94) - 설정 파일(`.properties`)을 활용한 메시지 관리와 국제화 서비스
- [검증 Validation](https://github.com/genesis12345678/TIL/blob/main/Spring/springmvc_2/validation/validation.md#%EA%B2%80%EC%A6%9D) - 요청에 대한 검증을 순수 코드부터 애노테이션 적용까지 점진적으로 알아보기
- [로그인 처리(1)](https://github.com/genesis12345678/TIL/blob/main/Spring/springmvc_2/login_1/login_1.md#%EB%A1%9C%EA%B7%B8%EC%9D%B8-%EC%B2%98%EB%A6%AC---%EC%BF%A0%ED%82%A4-%EC%84%B8%EC%85%98) - 쿠키와 세션으로 로그인 처리를 구현하면서 쿠키와 세션 알아보기
- [로그인 처리(2)](https://github.com/genesis12345678/TIL/blob/main/Spring/springmvc_2/login_2/login_2.md#%EB%A1%9C%EA%B7%B8%EC%9D%B8-%EC%B2%98%EB%A6%AC---%ED%95%84%ED%84%B0-%EC%9D%B8%ED%84%B0%EC%85%89%ED%84%B0) - 서블릿 필터와 스프링 인터셉터로 공통 관심사 해결
- [예외 처리와 오류 페이지](https://github.com/genesis12345678/TIL/blob/main/Spring/springmvc_2/exception_errorPage/exception_errorPage.md#%EC%98%88%EC%99%B8-%EC%B2%98%EB%A6%AC%EC%99%80-%EC%98%A4%EB%A5%98-%ED%8E%98%EC%9D%B4%EC%A7%80) - 애플리케이션에서 예외가 발생했을 때 과정과 오류 페이지 관리
- [API 예외 처리](https://github.com/genesis12345678/TIL/blob/main/Spring/springmvc_2/api_exception/api_exception.md#api-%EC%98%88%EC%99%B8-%EC%B2%98%EB%A6%AC) - API 예외 처리를 순수 코드부터 애노테이션 적용까지 점진적으로 알아보기
- [스프링 타입 컨터버](https://github.com/genesis12345678/TIL/blob/main/Spring/springmvc_2/typeConverter/typeConverter.md#%EC%8A%A4%ED%94%84%EB%A7%81-%ED%83%80%EC%9E%85-%EC%BB%A8%EB%B2%84%ED%84%B0) - 컨터버와 포맷터에 대해
- [파일 업로드](https://github.com/genesis12345678/TIL/blob/main/Spring/springmvc_2/fileUpload/fileUpload.md#%ED%8C%8C%EC%9D%BC-%EC%97%85%EB%A1%9C%EB%93%9C) - 서블릿과 스프링으로 파일 업로드 해보기

</details>

</details>

<details>
    <summary>스프링 DB</summary>
<details>
    <summary>1편</summary>

- [메인](https://github.com/genesis12345678/TIL/blob/main/Spring/database_1/database_1.md#%EC%8A%A4%ED%94%84%EB%A7%81-db-1%ED%8E%B8)
- [JDBC](https://github.com/genesis12345678/TIL/blob/main/Spring/database_1/database_1.md#jdbc) - JDBC에 대해
- [커넥션 풀과 데이터 소스]() - 커넥션 풀과 데이터 소스(`DataSource`)에 대해
- [트랜잭션](https://github.com/genesis12345678/TIL/blob/main/Spring/database_1/transaction/transaction.md#%ED%8A%B8%EB%9E%9C%EC%9E%AD%EC%85%98) - 트랜잭션 개념과 트랜잭션 적용 해보기
- [스프링 트랜잭션](https://github.com/genesis12345678/TIL/blob/main/Spring/database_1/spring_transaction/spring_transaction.md#%EC%8A%A4%ED%94%84%EB%A7%81%EA%B3%BC-%EB%AC%B8%EC%A0%9C-%ED%95%B4%EA%B2%B0---%ED%8A%B8%EB%9E%9C%EC%9E%AD%EC%85%98) - 트랜잭션을 적용했을 때 문제점을 스프링으로 해결해보기
- [자바 예외](https://github.com/genesis12345678/TIL/blob/main/Spring/database_1/javaException/javaException.md#%EC%9E%90%EB%B0%94-%EC%98%88%EC%99%B8) - 자바의 예외에 대해(체크, 언체크 예외)
- [스프링 예외 처리](https://github.com/genesis12345678/TIL/blob/main/Spring/database_1/springException/springException.md#%EC%8A%A4%ED%94%84%EB%A7%81%EA%B3%BC-%EB%AC%B8%EC%A0%9C-%ED%95%B4%EA%B2%B0---%EC%98%88%EC%99%B8-%EC%B2%98%EB%A6%AC-%EB%B0%98%EB%B3%B5) - 스프링에서 예외 추상화를 하는 방법

</details>

<details>
    <summary>2편</summary>

- [메인](https://github.com/genesis12345678/TIL/blob/main/Spring/database_2/db2.md#db2---%EB%8D%B0%EC%9D%B4%ED%84%B0-%EC%A0%91%EA%B7%BC-%EA%B8%B0%EC%88%A0)
- [JdbcTemplate](https://github.com/genesis12345678/TIL/blob/main/Spring/database_2/jdbcTemplate/jdbcTemplate.md#jdbctemplate) - `JdbcTemplate` 구현하면서 알아보기
- [MyBatis](https://github.com/genesis12345678/TIL/blob/main/Spring/database_2/myBaits/myBatis.md#mybatis) - `MyBatis` 구현하면서 알아보기
- [JPA](https://github.com/genesis12345678/TIL/blob/main/Spring/database_2/jpa/jpa.md#jpa) - `JPA` 구현하면서 알아보기
- [스프링 데이터 JPA](https://github.com/genesis12345678/TIL/blob/main/Spring/database_2/springJpa/springJpa.md#%EC%8A%A4%ED%94%84%EB%A7%81-%EB%8D%B0%EC%9D%B4%ED%84%B0-jpa) - `스프링 데이터 JPA` 구현하면서 알아보기
- [Querydsl](https://github.com/genesis12345678/TIL/blob/main/Spring/database_2/querydsl/querydsl.md#querydsl) - `Querydsl` 구현하면서 알아보기
- [테스트](https://github.com/genesis12345678/TIL/blob/main/Spring/database_2/test/dbTest.md#db-%EC%A0%91%EA%B7%BC---%ED%85%8C%EC%8A%A4%ED%8A%B8) - 테스트 코드에서 DB 접근에 대해
- [활용 방안](https://github.com/genesis12345678/TIL/blob/main/Spring/database_2/tradeOff/tradeOff.md#%ED%99%9C%EC%9A%A9-%EB%B0%A9%EC%95%88) - `스프링 데이터 JPA`와 `Querydsl`을 같이 사용할 때 트레이드 오프
- [스프링 트랜잭션](https://github.com/genesis12345678/TIL/blob/main/Spring/database_2/transaction/transaction.md#%EC%8A%A4%ED%94%84%EB%A7%81-%ED%8A%B8%EB%9E%9C%EC%9E%AD%EC%85%98-%EC%9D%B4%ED%95%B4) - 스프링의 트랜잭션에 대해 더 알아보기
- [트랜잭션 전파(1)](https://github.com/genesis12345678/TIL/blob/main/Spring/database_2/propagation/tx_propagation_1/tx_propagation.md#%EC%8A%A4%ED%94%84%EB%A7%81-%ED%8A%B8%EB%9E%9C%EC%9E%AD%EC%85%98-%EC%A0%84%ED%8C%8C-1) - 트랜잭션 전파에 대해
- [트랜잭션 전파(2)](https://github.com/genesis12345678/TIL/blob/main/Spring/database_2/propagation/tx_propagation_2/tx_propagation.md#%EC%8A%A4%ED%94%84%EB%A7%81-%ED%8A%B8%EB%9E%9C%EC%9E%AD%EC%85%98-%EC%A0%84%ED%8C%8C-2) - 트랜잭션 전파 활용
</details>
</details>

<details>
    <summary>스프링 부트</summary>

- [메인](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/SpringBoot.md#%EC%8A%A4%ED%94%84%EB%A7%81-%EB%B6%80%ED%8A%B8)
- [웹 서버와 서블릿 컨테이너](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/servletContainer/ServletContainer.md#%EC%9B%B9-%EC%84%9C%EB%B2%84%EC%99%80-%EC%84%9C%EB%B8%94%EB%A6%BF-%EC%BB%A8%ED%85%8C%EC%9D%B4%EB%84%88) - 스프링 부트가 없는 과거 버전으로 개발해보기
- [내장 톰캣](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/embedTomcat/EmbedTomcat.md#%EB%82%B4%EC%9E%A5-%ED%86%B0%EC%BA%A3) - 내장 톰캣을 사용하여 여러 문제점들을 해결하고 스프링 부트 접목해보기
- [스프링 부트 스타터](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/starterLibrary/Library.md#%EC%8A%A4%ED%94%84%EB%A7%81-%EB%B6%80%ED%8A%B8-%EC%8A%A4%ED%83%80%ED%84%B0) - 스프링 부트가 라이브러리 버전 관리를 하는 방법
- [스프링 부트의 자동 구성](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/autoConfig/AutoConfig.md#%EC%9E%90%EB%8F%99-%EA%B5%AC%EC%84%B1) - 스프링 부트의 자동 구성에 대해
  - [자동 구성(1)](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/autoConfig/AutoConfig.md#%EC%8A%A4%ED%94%84%EB%A7%81-%EB%B6%80%ED%8A%B8%EC%9D%98-%EC%9E%90%EB%8F%99-%EA%B5%AC%EC%84%B1) - 자동 구성을 직접 만들어보고 자동 구성 이해하기
  - [자동 구성(2)](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/autoConfig/SpringBootAutoConfig_2.md#%EC%8A%A4%ED%94%84%EB%A7%81-%EB%B6%80%ED%8A%B8%EC%9D%98-%EC%9E%90%EB%8F%99-%EA%B5%AC%EC%84%B1) - 라이브러리를 직접 만들어보고 자동 구성 이해하기
- [외부 설정과 프로필](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/externalConfig/ExternalConfig.md#%EC%99%B8%EB%B6%80-%EC%84%A4%EC%A0%95) - 외부 설정으로 데이터를 관리하는 방법
  - [OS 환경 변수](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/externalConfig/OS.md#%EC%99%B8%EB%B6%80-%EC%84%A4%EC%A0%95---os-%ED%99%98%EA%B2%BD-%EB%B3%80%EC%88%98) - OS 환경 변수 사용법
  - [자바 시스템 속성](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/externalConfig/JavaSystem.md#%EC%99%B8%EB%B6%80-%EC%84%A4%EC%A0%95---%EC%9E%90%EB%B0%94-%EC%8B%9C%EC%8A%A4%ED%85%9C-%EC%86%8D%EC%84%B1) - 자바 시스템 속성 사용법
  - [커맨드 라인 인수](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/externalConfig/CommandLine.md#%EC%99%B8%EB%B6%80-%EC%84%A4%EC%A0%95---%EC%BB%A4%EB%A7%A8%EB%93%9C-%EB%9D%BC%EC%9D%B8-%EC%9D%B8%EC%88%98) - 커맨드 라인 인수 사용법
  - [스프링 통합](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/externalConfig/SpringCombine.md#%EC%8A%A4%ED%94%84%EB%A7%81-%ED%86%B5%ED%95%A9) - 여러 외부 설정 값에 따라서 스프링이 데이터를 읽는 방법
  - [설정 데이터](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/externalConfig/ExternalFile.md#%EC%84%A4%EC%A0%95-%EB%8D%B0%EC%9D%B4%ED%84%B0---%EC%99%B8%EB%B6%80-%ED%8C%8C%EC%9D%BC) - 설정 데이터(`.properties`) 외부 파일과 내부 파일, 우선순위에 대해
  - [외부 설정 사용](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/externalConfig/ExternalRead.md#%EC%99%B8%EB%B6%80-%EC%84%A4%EC%A0%95-%EC%82%AC%EC%9A%A9) - `@Value`와 `@ConfigurationProperties`에 대해
  - [YAML](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/externalConfig/YAML.md#yaml) - `.yml`에 대해
  - [@Profile](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/externalConfig/%40Profile.md#profile) - `@Profile`에 대해
- [액츄에이터](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/actuator/Actuator.md#%EC%95%A1%EC%B8%84%EC%97%90%EC%9D%B4%ED%84%B0) - 스프링 부트 액츄에이터에 대해
  - [시작](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/actuator/Basic.md#%EC%95%A1%EC%B8%84%EC%97%90%EC%9D%B4%ED%84%B0-%EC%8B%9C%EC%9E%91) - 액츄에이터 기본 사용법과 엔드포인트
  - [헬스 정보](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/actuator/Health.md#%ED%97%AC%EC%8A%A4-%EC%A0%95%EB%B3%B4) - 액츄에이터 헬스 정보에 대해
  - [애플리케이션 정보](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/actuator/Info.md#%EC%95%A0%ED%94%8C%EB%A6%AC%EC%BC%80%EC%9D%B4%EC%85%98-%EC%A0%95%EB%B3%B4) - 액츄에이터 애플리케이션 정보에 대해
  - [로거](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/actuator/Logger.md#%EB%A1%9C%EA%B1%B0) - 액츄에이션 로거 정보에 대해
  - [HTTP 요청 응답 기록](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/actuator/HttpExchange.md#http-%EC%9A%94%EC%B2%AD-%EC%9D%91%EB%8B%B5-%EA%B8%B0%EB%A1%9D) - 액츄에이터 HTTP 요청 응답 기록에 대해
  - [보안](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/actuator/Security.md#%EC%95%A1%EC%B8%84%EC%97%90%EC%9D%B4%ED%84%B0-%EB%B3%B4%EC%95%88) - 액츄에이터 보안 유의점
- [마이크로미터](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/monitoring/micrometer.md#%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%EB%AF%B8%ED%84%B0) - 마이크로미터와 메트릭에 대해
  - [프로메테우스](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/monitoring/Prometheus.md#%ED%94%84%EB%A1%9C%EB%A9%94%ED%85%8C%EC%9A%B0%EC%8A%A4) - 프로메테우스 기본 사용법과 기본 기능
  - [그라파나](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/SpringBoot.md#%EA%B7%B8%EB%9D%BC%ED%8C%8C%EB%82%98) - 그라파나 기본 사용법
- [모니터링 메트릭 활용](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/monitoring/MetricsUse.md#%EB%AA%A8%EB%8B%88%ED%84%B0%EB%A7%81-%EB%A9%94%ED%8A%B8%EB%A6%AD-%ED%99%9C%EC%9A%A9) - 비즈니스 메트릭 등록해보기, 실무 모니터링 팁
  - [카운터](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/monitoring/Counter.md#%EB%A9%94%ED%8A%B8%EB%A6%AD-%EB%93%B1%EB%A1%9D---%EC%B9%B4%EC%9A%B4%ED%84%B0) - 카운터 메트릭 등록
    - [V1](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/monitoring/Counter.md#%EC%B9%B4%EC%9A%B4%ED%84%B0---v1) - 코드로 만들기
    - [V2](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/monitoring/Counter.md#%EC%B9%B4%EC%9A%B4%ED%84%B0---v2) - 애노테이션 적용
  - [타이머](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/monitoring/Timer.md#%EB%A9%94%ED%8A%B8%EB%A6%AD-%EB%93%B1%EB%A1%9D---%ED%83%80%EC%9D%B4%EB%A8%B8) - 타이머 메트릭 등록
    - [V1](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/monitoring/Timer.md#%ED%83%80%EC%9D%B4%EB%A8%B8---v1) - 코드로 만들기
    - [V2](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/monitoring/Timer.md#%ED%83%80%EC%9D%B4%EB%A8%B8---v2) - 애노테이션 적용
  - [게이지](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/monitoring/Gauge.md#%EB%A9%94%ED%8A%B8%EB%A6%AD-%EB%93%B1%EB%A1%9D---%EA%B2%8C%EC%9D%B4%EC%A7%80) - 게이지 메트릭 등록
    - [V1](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/monitoring/Gauge.md#%EA%B2%8C%EC%9D%B4%EC%A7%80---v1) - 코드로 만들기
    - [V2](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/monitoring/Gauge.md#%EA%B2%8C%EC%9D%B4%EC%A7%80---v2) - 간단한 버전
</details>

### JPA

<details>
    <summary>기본</summary>

- [메인](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/jpa.md#jpa)
- [영속성 컨텍스트](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/persistenceContext/persistenceContext.md#%EC%98%81%EC%86%8D%EC%84%B1-%EA%B4%80%EB%A6%AC) - 영속성 컨텍스트에 대한 용어 이해
- [엔티티 매핑](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/entityMapping/entityMapping.md#%EC%97%94%ED%8B%B0%ED%8B%B0-%EB%A7%A4%ED%95%91) - 엔티티와 테이블 매핑 기본
- [연관 관계 매핑](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/related/related.md#%EC%97%B0%EA%B4%80-%EA%B4%80%EA%B3%84-%EB%A7%A4%ED%95%91) - 단방향, 양방향, 연관관계의 주인에 대해
- [다양한 연관 관계 매핑](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/related/relateds.md#%EB%8B%A4%EC%96%91%ED%95%9C-%EC%97%B0%EA%B4%80%EA%B4%80%EA%B3%84) - 일대일, 다대일 등의 연관관계에 대해
- [고급 매핑](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/inheritance/inheritance.md#%EC%83%81%EC%86%8D%EA%B4%80%EA%B3%84-%EB%A7%A4%ED%95%91) - 테이블 상속 구현하기
- [프록시](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/proxy/proxy.md#%ED%94%84%EB%A1%9D%EC%8B%9C) - JPA의 프록시 기술, 즉시 로딩과 지연 로딩, 영속성 전이에 대해
- [값 타입](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/valueType/valueType.md#%EA%B0%92-%ED%83%80%EC%9E%85) - 임베디드 타입과 불변 객체, 값 타입 컬렉션에 대해
- [JPQL(1)](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/jpql/jpql.md#jpql) - `JPQL` 기본 사용법
- [JPQL(2)](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/jpql/jpql_2.md#jpql) - `JPQL` 심화 사용법

</details>

<details>
  <summary>JPA를 활용한 웹 애플리케이션 개발 - 1</summary>

- [메인](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/use_1/Use.md#jpa%EB%A5%BC-%ED%99%9C%EC%9A%A9%ED%95%9C-%EC%9B%B9-%EC%95%A0%ED%94%8C%EB%A6%AC%EC%BC%80%EC%9D%B4%EC%85%98-%EA%B0%9C%EB%B0%9C)
- [엔티티 개발](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/use_1/entity/Design.md#%EC%84%A4%EA%B3%84) - 엔티티 클래스 개발 및 엔티티 설계 시 주의할 점
- [도메인 개발](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/use_1/domain/Domain.md#%EB%8F%84%EB%A9%94%EC%9D%B8-%EA%B0%9C%EB%B0%9C) - 레포지토리 및 서비스 계층 개발
- [웹 계층 개발](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/use_1/web/Web.md#%EC%9B%B9-%EA%B3%84%EC%B8%B5-%EA%B0%9C%EB%B0%9C) - 웹 계층 개발 및 **변경 감지와 병합**에 대해
</details>

<details>
  <summary>JPA를 활용한 웹 애플리케이션 개발 - 2</summary>

- [메인](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/use_2/Use.md#jpa%EB%A5%BC-%ED%99%9C%EC%9A%A9%ED%95%9C-%EC%9B%B9-%EC%95%A0%ED%94%8C%EB%A6%AC%EC%BC%80%EC%9D%B4%EC%85%98-%EA%B0%9C%EB%B0%9C)
- [API 조회 기본](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/use_2/Basic.md#%ED%9A%8C%EC%9B%90-api) - 기본적인 등록, 수정, 조회 API
- [지연 로딩과 조회 성능 최적화](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/use_2/OptimizingInquiry.md#%EC%A7%80%EC%97%B0-%EB%A1%9C%EB%94%A9%EA%B3%BC-%EC%A1%B0%ED%9A%8C-%EC%84%B1%EB%8A%A5-%EC%B5%9C%EC%A0%81%ED%99%94) - `XToOne` 연관관계 조회 성능 최적화
  - [V1](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/use_2/OptimizingInquiry.md#%EC%A3%BC%EB%AC%B8-%EC%A1%B0%ED%9A%8C---v1) - 엔티티 직접 노출
  - [V2](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/use_2/OptimizingInquiry.md#%EC%A3%BC%EB%AC%B8-%EC%A1%B0%ED%9A%8C---v2) - 엔티티 DTO 변환
  - [V3](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/use_2/OptimizingInquiry.md#%EC%A3%BC%EB%AC%B8-%EC%A1%B0%ED%9A%8C---v3) - DTO로 변환 후 페치 조인 적용
  - [V4](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/use_2/OptimizingInquiry.md#%EC%A3%BC%EB%AC%B8-%EC%A1%B0%ED%9A%8C---v4) - DTO로 바로 조회
  - [정리](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/use_2/OptimizingInquiry.md#%EC%A0%95%EB%A6%AC)
- [컬렉션 조회 성능 최적화](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/use_2/CollectionOptimizing.md#%EC%BB%AC%EB%A0%89%EC%85%98-%EC%A1%B0%ED%9A%8C-%EC%B5%9C%EC%A0%81%ED%99%94) - `XToMany` 연관관계 조회 성능 최적화
  - [V1](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/use_2/CollectionOptimizing.md#%EC%A1%B0%ED%9A%8C---v1) - 엔티티 직접 노출
  - [V2](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/use_2/CollectionOptimizing.md#%EC%A1%B0%ED%9A%8C---v2) - 엔티티 DTO 변환
  - [V3](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/use_2/CollectionOptimizing.md#%EC%A1%B0%ED%9A%8C---v3) - DTO로 변환 후 페치 조인 적용(페이징 불가능)
  - [V3.1](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/use_2/CollectionOptimizing.md#%EC%A1%B0%ED%9A%8C---v31) - `V3` 페이징 불가능 문제 해결
  - [V4](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/use_2/CollectionOptimizing.md#%EC%A1%B0%ED%9A%8C---v4) - DTO로 바로 조회(`N + 1`문제 발생)
  - [V5](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/use_2/CollectionOptimizing.md#%EC%A1%B0%ED%9A%8C---v5) - DTO로 바로 조회, 컬렉션 조회 최적화
  - [V6](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/use_2/CollectionOptimizing.md#%EC%A1%B0%ED%9A%8C---v6) - DTO로 바로 조회, 플랫 데이터 최적화
  - [정리](https://github.com/genesis12345678/TIL/blob/main/Spring/jpa/use_2/CollectionOptimizing.md#%EC%A0%95%EB%A6%AC)
- [OSIV]() - `OSIV`에 대해
</details>

<details>
    <summary>스프링 데이터 JPA</summary>

- [메인](https://github.com/genesis12345678/TIL/blob/main/Spring/dataJpa/spring_data_jpa.md#%EC%8A%A4%ED%94%84%EB%A7%81-%EB%8D%B0%EC%9D%B4%ED%84%B0-jpa)
- [공통 인터페이스](https://github.com/genesis12345678/TIL/blob/main/Spring/dataJpa/common_interface/common_interface.md#%EA%B3%B5%ED%86%B5-%EC%9D%B8%ED%84%B0%ED%8E%98%EC%9D%B4%EC%8A%A4-%EA%B8%B0%EB%8A%A5) - 스프링 데이터 JPA의 구조
- [쿼리 메서드 기능(1)](https://github.com/genesis12345678/TIL/blob/main/Spring/dataJpa/query_method/query_method_1.md#%EC%BF%BC%EB%A6%AC-%EB%A9%94%EC%84%9C%EB%93%9C-%EA%B8%B0%EB%8A%A5---1) - 메서드 이름으로 쿼리 생성, `@Query` 등에 대해
- [쿼리 메서드 기능(2)](https://github.com/genesis12345678/TIL/blob/main/Spring/dataJpa/query_method/query_method_2.md#%EC%BF%BC%EB%A6%AC-%EB%A9%94%EC%84%9C%EB%93%9C---2) - 페이징, `@EntityGraph`등에 대해
- [확장 기능](https://github.com/genesis12345678/TIL/blob/main/Spring/dataJpa/extend/extend.md#%ED%99%95%EC%9E%A5-%EA%B8%B0%EB%8A%A5) - 스프링 데이터 JPA를 확장하여 사용할 수 있는 기술들(`Auditing`, `Web`확장 등)
- [분석](https://github.com/genesis12345678/TIL/blob/main/Spring/dataJpa/analyse/analyse.md#%EC%8A%A4%ED%94%84%EB%A7%81-%EB%8D%B0%EC%9D%B4%ED%84%B0-jpa-%EB%B6%84%EC%84%9D) - 스프링 데이터 JPA가 사용하는 구현체와 새로운 엔티티를 구별하는 방법에 대해
- [그 외 기능들](https://github.com/genesis12345678/TIL/blob/main/Spring/dataJpa/functions/functions.md#%EC%8A%A4%ED%94%84%EB%A7%81-%EB%8D%B0%EC%9D%B4%ED%84%B0-jpa-%EB%82%98%EB%A8%B8%EC%A7%80-%EA%B8%B0%EB%8A%A5%EB%93%A4) - 프로젝션과 Native Query
</details>

<details>
    <summary>Querydsl</summary>

- [메인](https://github.com/genesis12345678/TIL/blob/main/Spring/querydsl/querydsl.md#querydsl)
- [기본 문법(1)](https://github.com/genesis12345678/TIL/blob/main/Spring/querydsl/basic/basic_1.md#querydsl-%EA%B8%B0%EB%B3%B8-%EB%AC%B8%EB%B2%95---1) - 검색, 결과 조회, 정렬, 페이징
- [기본 문법(2)](https://github.com/genesis12345678/TIL/blob/main/Spring/querydsl/basic/basic_2.md#querydsl-%EA%B8%B0%EB%B3%B8-%EB%AC%B8%EB%B2%95---2) - 집합 함수, 조인, 페치 조인
- [기본 문법(3)](https://github.com/genesis12345678/TIL/blob/main/Spring/querydsl/basic/basic_3.md#querydsl-%EA%B8%B0%EB%B3%B8-%EB%AC%B8%EB%B2%95---3) - 서브 쿼리, `Case`문
- [중급 문법(1)](https://github.com/genesis12345678/TIL/blob/main/Spring/querydsl/intermidate/intermediate_1.md#querydsl-%EC%A4%91%EA%B8%89-%EB%AC%B8%EB%B2%95---1) - 프로젝션 결과 반환의 여러가지 방법
- [중급 문법(2)](https://github.com/genesis12345678/TIL/blob/main/Spring/querydsl/intermidate/intermediate_2.md#querydsl-%EC%A4%91%EA%B8%89-%EB%AC%B8%EB%B2%95---2) - 동적 쿼리, 벌크 연산
</details>


### CS 💻

<details>
  <summary>HTTP</summary>

- [메인](https://github.com/genesis12345678/TIL/blob/main/Http/HTTP.md#http-%EA%B8%B0%EB%B3%B8-%EC%A7%80%EC%8B%9D)
- [인터넷 네트워크](https://github.com/genesis12345678/TIL/blob/main/Http/network/network.md#ip---%EC%9D%B8%ED%84%B0%EB%84%B7-%ED%94%84%EB%A1%9C%ED%86%A0%EC%BD%9C) - `IP`, `TCP와 UDP`, `PORT`, `DNS`에 대해
- [URI](https://github.com/genesis12345678/TIL/blob/main/Http/uri/uri.md#uri) - `URI`와 웹 브라우저 요청의 흐름
- [Http](https://github.com/genesis12345678/TIL/blob/main/Http/http/http.md#http) - `Http` 특징에 대해
- [Http 메서드](https://github.com/genesis12345678/TIL/blob/main/Http/httpMethod/httpMethod.md#http-method) - `Http` 메서드와 API 설계 예시
- [Http 상태코드](https://github.com/genesis12345678/TIL/blob/main/Http/httpStatusCode/httpStatusCode.md#http-%EC%83%81%ED%83%9C-%EC%BD%94%EB%93%9C) - 여러가지 `Http` 상태코드에 대해
- [Http 일반헤더](https://github.com/genesis12345678/TIL/blob/main/Http/httpHeader_1/header_1.md#http-%EC%9D%BC%EB%B0%98-%ED%97%A4%EB%8D%94) - `Http` 헤더의 표현, 협상, 전송 방식, 정보, 인증, 쿠키에 대해
- [Http 헤더(Cache)](https://github.com/genesis12345678/TIL/blob/main/Http/httpHeader_2/httpHeader_2.md#http-%ED%97%A4%EB%8D%94---cache) - `Http` 헤더의 캐시(`Cache`)에 대해

</details>

<details>
  <summary>OS</summary>

- [PCB](https://github.com/genesis12345678/TIL/blob/main/OS/PCB_and_ContextSwitching/pcb.md#pcb--context-switching) - `PCB`와 `컨텍스트 스위칭`에 대해
- [CPU Scheduling](https://github.com/genesis12345678/TIL/blob/main/OS/cpuScheduling/Scheduling.md#cpu-scheduling) - `CPU 스케줄링`에 대해(`FCFS`, `SJF` 등)
- [Memory](https://github.com/genesis12345678/TIL/blob/main/OS/memory/memory.md#memory---%EB%A9%94%EB%AA%A8%EB%A6%AC) - `Memory` 영역에 대해
- [OS](https://github.com/genesis12345678/TIL/blob/main/OS/os/OperatingSystem.md#os---%EC%9A%B4%EC%98%81%EC%B2%B4%EC%A0%9C) - 운영체제(`OS`)에 대해
- [Process](https://github.com/genesis12345678/TIL/blob/main/OS/process/process.md#process---%ED%94%84%EB%A1%9C%EC%84%B8%EC%8A%A4) - `Process`, `Thread`, `멀티 태스킹`에 대해

</details>

### 자료구조 📊

- [자료구조란?](https://github.com/genesis12345678/TIL/blob/main/dataStructure/dataStructure/dataStructure.md#%EC%9E%90%EB%A3%8C-%EA%B5%AC%EC%A1%B0)

<details>
  <summary>선형 자료구조</summary>

- [배열](https://github.com/genesis12345678/TIL/blob/main/dataStructure/linear/Array/Array.md#array---%EB%B0%B0%EC%97%B4) - `Array`와 `ArrayList`에 대해
  - [`ArrayList` 직접 구현해보기](https://github.com/genesis12345678/TIL/blob/main/dataStructure/linear/Array/ArrayList.java)
- [연결 리스트](https://github.com/genesis12345678/TIL/blob/main/dataStructure/linear/linkedList/LinkedList.md#linkedlist) - `LinkedList`에 대해
  - [`SingleLinkedList` 직접 구현해보기](https://github.com/genesis12345678/TIL/blob/main/dataStructure/linear/linkedList/singleLinkedList/SinglyLinkedList.java)
  - [`DoubleLinkedList` 직접 구현해보기](https://github.com/genesis12345678/TIL/blob/main/dataStructure/linear/linkedList/doubleLinkedList/DoublyLinkedList.java#L20)
- [스택](https://github.com/genesis12345678/TIL/blob/main/dataStructure/linear/stack/Stack.md#stack---%EC%8A%A4%ED%83%9D) - `Stack`에 대해
  - [`LinkedStack` 직접 구현해보기](https://github.com/genesis12345678/TIL/blob/main/dataStructure/linear/stack/linkedStack/LinkedStack.java)
  - [`ArrayStack` 직접 구현해보기](https://github.com/genesis12345678/TIL/blob/main/dataStructure/linear/stack/arrayStack/ArrayStack.java)
- [큐](https://github.com/genesis12345678/TIL/blob/main/dataStructure/linear/queue/Queue.md#queue---%ED%81%90) - `Queue`에 대해
  - [`LinkedtQueue` 직접 구현해보기](https://github.com/genesis12345678/TIL/blob/main/dataStructure/linear/queue/linkedQueue/LinkedListQueue.java)
  - [`ArrayQueue` 직접 구현해보기](https://github.com/genesis12345678/TIL/blob/main/dataStructure/linear/queue/arrayQueue/ArrayQueue.java)
- [데크](https://github.com/genesis12345678/TIL/blob/main/dataStructure/linear/dequeue/Deque.md#deque-%EB%8D%B0%ED%81%AC) - `Deque`에 대해
  - [`LinkedDeque` 직접 구현해보기](https://github.com/genesis12345678/TIL/blob/main/dataStructure/linear/dequeue/linkedDeque/LinkedDeque.java)
  - [`ArrayDeque` 직접 구현해보기](https://github.com/genesis12345678/TIL/blob/main/dataStructure/linear/dequeue/arrayDeque/ArrayDeque.java)
- [해시 테이블](https://github.com/genesis12345678/TIL/blob/main/dataStructure/linear/hash/hash.md#%ED%95%B4%EC%8B%9Chash) - `Hash`에 대해
  - [`HashSet` 직접 구현해보기](https://github.com/genesis12345678/TIL/blob/main/dataStructure/linear/hash/hashSet/HashSet.java)

</details>

<details>
  <summary>비선형 자료구조</summary>

- [그래프](https://github.com/genesis12345678/TIL/blob/main/dataStructure/non_linear/graph/graph.md#%EA%B7%B8%EB%9E%98%ED%94%84) - `Graph`와 `트리`에 대해
  - [인접 행렬 방식 예제](https://github.com/genesis12345678/TIL/blob/main/dataStructure/non_linear/graph/ArrayGraph.java)
  - [인접 리스트 방식 예제](https://github.com/genesis12345678/TIL/blob/main/dataStructure/non_linear/graph/LinkedGraph.java)
- [힙](https://github.com/genesis12345678/TIL/blob/main/dataStructure/non_linear/heap/heap.md#heap---%ED%9E%99) - `Heap`에 대해
  - [최소힙(`MinHeap`) 직접 구현해보기](https://github.com/genesis12345678/TIL/blob/main/dataStructure/non_linear/heap/minHeap/MinHeap.java)
  - [최대힙(`MaxHeap`) 직접 구현해보기](https://github.com/genesis12345678/TIL/blob/main/dataStructure/non_linear/heap/maxHeap/MaxHeap.java)

</details>

### GIT

- [메인](https://github.com/genesis12345678/TIL/blob/main/git/Main.md#git)
<details>
  <summary>기본</summary>

- [초반 설정](https://github.com/genesis12345678/TIL/blob/main/git/Start.md#git-%EC%B5%9C%EC%B4%88-%EC%84%A4%EC%A0%95) - `Git`을 사용할 때 최초로 하는 설정(`config`와 `.gitignore`)
- [변경사항 저장](https://github.com/genesis12345678/TIL/blob/main/git/Save.md#%EB%B3%80%EA%B2%BD%EC%82%AC%ED%95%AD-%EC%A0%80%EC%9E%A5%ED%95%98%EA%B8%B0) - 변경사항을 커밋하기
</details>

<details>
  <summary>Branch</summary>

- [기본적인 브랜치 다루는 방법](https://github.com/genesis12345678/TIL/blob/main/git/Branch.md#branch) - 생성, 확인, 이동, 삭제 등
- [브랜치 합치기](https://github.com/genesis12345678/TIL/blob/main/git/Branch.md#%EB%B8%8C%EB%9E%9C%EC%B9%98-%ED%95%A9%EC%B9%98%EA%B8%B0) - `merge`와 `rebase`
- [Git의 merge 전략](https://github.com/genesis12345678/TIL/blob/main/git/Branch.md#git%EC%9D%98-merge-%EC%A0%84%EB%9E%B5) - `fast-forward`, `3-way merge`, 다양한 `merge` 옵션들에 대해
- [다른 브랜치](https://github.com/genesis12345678/TIL/blob/main/git/Branch.md#%EB%8B%A4%EB%A5%B8-%EB%B8%8C%EB%9E%9C%EC%B9%98%EC%97%90%EC%84%9C-%EC%9B%90%ED%95%98%EB%8A%94-%EC%BB%A4%EB%B0%8B-%EA%B0%80%EC%A0%B8%EC%98%A4%EA%B8%B0) - 다른 브랜치에서 원하는 커밋 가져오기(`cherry-pick`), 파생된 브랜치 옮겨붙이기(`rebase --onto`), 커밋들 하나로 묶어 가져오기(`--squash`)
- [Gitflow](https://github.com/genesis12345678/TIL/blob/main/git/Branch.md#gitflow) - 협업을 위한 브랜칭 전략

</details>

<details>
  <summary>되돌리기</summary>

- [과거로 가기](https://github.com/genesis12345678/TIL/blob/main/git/Past.md#%EA%B3%BC%EA%B1%B0%EB%A1%9C-%EA%B0%80%EA%B8%B0) - `reset`과 `revert`
- [취소와 되돌리기](https://github.com/genesis12345678/TIL/blob/main/git/Revert.md#%EC%B7%A8%EC%86%8C%EC%99%80-%EB%90%98%EB%8F%8C%EB%A6%AC%EA%B8%B0) - `Git`에서 관리되지 않는 파일들 삭제, 커밋하지 않은 변경사항 되돌리기, `reset` 복구하기
</details>

<details>
  <summary>Git 더 알아보기</summary>

- [Git의 3가지 공간](https://github.com/genesis12345678/TIL/blob/main/git/Deep.md#git%EC%9D%98-3%EA%B0%80%EC%A7%80-%EA%B3%B5%EA%B0%84) - `Git`이 파일을 관리하는 방법에 대해(+`reset`의 3가지 옵션)
- [HEAD](https://github.com/genesis12345678/TIL/blob/main/git/Deep.md#git%EC%9D%98-head) - `HEAD`라는 개념을 활용하는 방법
- [fetch vs pull](https://github.com/genesis12345678/TIL/blob/main/git/Deep.md#fetch%EC%99%80-pull) - `fetch`와 `pull`의 차이점
- [Help](https://github.com/genesis12345678/TIL/blob/main/git/Deep.md#git-help) - `Git help`에 대해
- [Config](https://github.com/genesis12345678/TIL/blob/main/git/Deep.md#git-config) - 설정값 보기, 단축키 설정 등 `Git config` 관련 명령어

</details>

<details>
  <summary>원격 저장소</summary>

- [원격 저장소](https://github.com/genesis12345678/TIL/blob/main/git/GitHub.md#%EC%9B%90%EA%B2%A9-%EC%A0%80%EC%9E%A5%EC%86%8Cgithub) - `GitHub`에 대해
  - 로컬과 원격 연결
  - 원격 저장소에서 프로젝트 가져오기
  - `pull`을 하는 두 가지 방법

</details>

<details>
  <summary>커밋 관리</summary>

- [커밋 권장사항](https://github.com/genesis12345678/TIL/blob/main/git/Commit.md#%EC%9E%91%EC%97%85%EC%9D%84-%EC%BB%A4%EB%B0%8B%ED%95%A0-%EB%95%8C-%EA%B6%8C%EC%9E%A5%EC%82%AC%ED%95%AD) - 커밋 권장사항 및 컨벤션
- [세심하게 커밋](https://github.com/genesis12345678/TIL/blob/main/git/Commit.md#%EC%84%B8%EC%8B%AC%ED%95%98%EA%B2%8C-%EC%8A%A4%ED%85%8C%EC%9D%B4%EC%A7%95-%ED%95%98%EA%B3%A0-%EC%BB%A4%EB%B0%8B%ED%95%98%EA%B8%B0) - `hunk`별 스테이징 진행
- [커밋 치워두기](https://github.com/genesis12345678/TIL/blob/main/git/Commit.md#%EC%BB%A4%EB%B0%8B%ED%95%98%EA%B8%B0-%EC%95%A0%EB%A7%A4%ED%95%9C-%EB%B3%80%ED%99%94-%EC%B9%98%EC%9B%8C%EB%91%90%EA%B8%B0) - `stash`에 대해
- [커밋 수정하기](https://github.com/genesis12345678/TIL/blob/main/git/Commit.md#%EC%BB%A4%EB%B0%8B-%EC%88%98%EC%A0%95%ED%95%98%EA%B8%B0) - 과거 커밋 내역을 수정하는 방법
- [태그](https://github.com/genesis12345678/TIL/blob/main/git/Commit.md#%EC%BB%A4%EB%B0%8B-%ED%83%9C%EA%B7%B8) - `Git`의 `Tag`에 대해

</details>

<details>
  <summary>분석과 디버깅</summary>

- [log](https://github.com/genesis12345678/TIL/blob/main/git/Debug.md#log) - `git log`의 다양한 옵션들
- [차이 살펴보기](https://github.com/genesis12345678/TIL/blob/main/git/Debug.md#%EC%B0%A8%EC%9D%B4-%EC%82%B4%ED%8E%B4%EB%B3%B4%EA%B8%B0) - 파일, 커밋, 브랜치의 차이를 CLI로 알아보는 방법
- [오류 발생지점 찾기](https://github.com/genesis12345678/TIL/blob/main/git/Debug.md#%EC%98%A4%EB%A5%98-%EB%B0%9C%EC%83%9D-%EC%8B%9C%EC%A0%90-%EC%B0%BE%EA%B8%B0) - `git`으로 오류가 발생하는 커밋 지점을 찾는 방법

</details>

### Algorithm 

- [시간 복잡도](https://github.com/genesis12345678/TIL/blob/main/algorithm/Algorithm.md#%EC%8B%9C%EA%B0%84-%EB%B3%B5%EC%9E%A1%EB%8F%84-%ED%91%9C%EA%B8%B0%EB%B2%95) - 시간 복잡도 표기법과 활용에 대해

<details>
  <summary>자료구조</summary>

- [배열과 리스트](https://github.com/genesis12345678/TIL/blob/main/algorithm/dataStructure/array/List.md#%EB%B0%B0%EC%97%B4%EA%B3%BC-%EB%A6%AC%EC%8A%A4%ED%8A%B8) - 배열과 리스트 자료구조
  - [예제 문제 - 1](https://github.com/genesis12345678/TIL/blob/main/algorithm/dataStructure/array/Example_1.md#%EB%B0%B0%EC%97%B4%EA%B3%BC-%EB%A6%AC%EC%8A%A4%ED%8A%B8-%EC%98%88%EC%A0%9C---1)
  - [예제 문제 - 2](https://github.com/genesis12345678/TIL/blob/main/algorithm/dataStructure/array/Example_2.md#%EB%B0%B0%EC%97%B4%EA%B3%BC-%EB%A6%AC%EC%8A%A4%ED%8A%B8-%EC%98%88%EC%A0%9C---1)
- [구간 합](https://github.com/genesis12345678/TIL/blob/main/algorithm/dataStructure/sectionSum/Section.md#%EA%B5%AC%EA%B0%84-%ED%95%A9) - 합 배열을 이용한 구간 합
  - [예제 문제 - 1](https://github.com/genesis12345678/TIL/blob/main/algorithm/dataStructure/sectionSum/Example_1.md#%EA%B5%AC%EA%B0%84-%ED%95%A9-%EC%98%88%EC%A0%9C---1)
  - [예제 문제 - 2](https://github.com/genesis12345678/TIL/blob/main/algorithm/dataStructure/sectionSum/Example_2.md#%EA%B5%AC%EA%B0%84-%ED%95%A9-%EC%98%88%EC%A0%9C---2)
  - [예제 문제 - 3](https://github.com/genesis12345678/TIL/blob/main/algorithm/dataStructure/sectionSum/Example_3.md#%EA%B5%AC%EA%B0%84-%ED%95%A9-%EC%98%88%EC%A0%9C---3)
- [투 포인터](https://github.com/genesis12345678/TIL/blob/main/algorithm/dataStructure/twoPointer/TwoPointer.md#%ED%88%AC-%ED%8F%AC%EC%9D%B8%ED%84%B0) - 두 개의 포인터로 시간 복잡도 최적화
  - [예제 문제 - 1](https://github.com/genesis12345678/TIL/blob/main/algorithm/dataStructure/twoPointer/Example_1.md#%ED%88%AC-%ED%8F%AC%EC%9D%B8%ED%84%B0-%EC%98%88%EC%A0%9C---1)
  - [예제 문제 - 2](https://github.com/genesis12345678/TIL/blob/main/algorithm/dataStructure/twoPointer/Example_2.md#%ED%88%AC-%ED%8F%AC%EC%9D%B8%ED%84%B0-%EC%98%88%EC%A0%9C---2)
  - [예제 문제 - 3](https://github.com/genesis12345678/TIL/blob/main/algorithm/dataStructure/twoPointer/Example_3.md#%ED%88%AC-%ED%8F%AC%EC%9D%B8%ED%84%B0-%EC%98%88%EC%A0%9C---3)
- [슬라이딩 윈도우](https://github.com/genesis12345678/TIL/blob/main/algorithm/dataStructure/slidingWindow/SlidingWindow.md#%EC%8A%AC%EB%9D%BC%EC%9D%B4%EB%94%A9-%EC%9C%88%EB%8F%84%EC%9A%B0) - 투 포인터 확장 개념
  - [예제 문제 - 1](https://github.com/genesis12345678/TIL/blob/main/algorithm/dataStructure/slidingWindow/Example_1.md#%EC%8A%AC%EB%9D%BC%EC%9D%B4%EB%94%A9-%EC%9C%88%EB%8F%84%EC%9A%B0-%EC%98%88%EC%A0%9C---1)
  - [예제 문제 - 2](https://github.com/genesis12345678/TIL/blob/main/algorithm/dataStructure/slidingWindow/Example_2.md#%EC%8A%AC%EB%9D%BC%EC%9D%B4%EB%94%A9-%EC%9C%88%EB%8F%84%EC%9A%B0-%EC%98%88%EC%A0%9C---2)
- [스택](https://github.com/genesis12345678/TIL/blob/main/algorithm/dataStructure/stack/Stack.md#%EC%8A%A4%ED%83%9D) - 스택 자료구조
  - [예제 문제 - 1](https://github.com/genesis12345678/TIL/blob/main/algorithm/dataStructure/stack/Example_1.md#%EC%8A%A4%ED%83%9D-%EC%98%88%EC%A0%9C---1)
  - [예제 문제 - 2](https://github.com/genesis12345678/TIL/blob/main/algorithm/dataStructure/stack/Example_2.md#%EC%8A%A4%ED%83%9D-%EC%98%88%EC%A0%9C---2)
- [큐](https://github.com/genesis12345678/TIL/blob/main/algorithm/dataStructure/queue/Queue.md#%ED%81%90) - 큐 자료구조
  - [예제 문제 - 1](https://github.com/genesis12345678/TIL/blob/main/algorithm/dataStructure/queue/Example_1.md#%ED%81%90-%EC%98%88%EC%A0%9C---1)
  - [예제 문제 - 2](https://github.com/genesis12345678/TIL/blob/main/algorithm/dataStructure/queue/Example_2.md#%ED%81%90-%EC%98%88%EC%A0%9C---2)
</details>

<details>
  <summary>정렬</summary>

- [버블 정렬](https://github.com/genesis12345678/TIL/blob/main/algorithm/sorting/bubbleSort/BubbleSort.md#%EB%B2%84%EB%B8%94-%EC%A0%95%EB%A0%AC) - `swap`, `O(n^2)`
  - [예제 문제 - 1](https://github.com/genesis12345678/TIL/blob/main/algorithm/sorting/bubbleSort/Example_1.md#%EB%B2%84%EB%B8%94-%EC%A0%95%EB%A0%AC-%EC%98%88%EC%A0%9C---1)
  - [예제 문제 - 2](https://github.com/genesis12345678/TIL/blob/main/algorithm/sorting/bubbleSort/Example_2.md#%EB%B2%84%EB%B8%94-%EC%86%8C%ED%8A%B8-%EC%98%88%EC%A0%9C---2)
- [선택 정렬](https://github.com/genesis12345678/TIL/blob/main/algorithm/sorting/selectionSort/SelectionSort.md#%EC%84%A0%ED%83%9D-%EC%A0%95%EB%A0%AC) - `O(n^2)`
  - [예제 문제 - 1](https://github.com/genesis12345678/TIL/blob/main/algorithm/sorting/selectionSort/Example_1.md#%EC%84%A0%ED%83%9D-%EC%A0%95%EB%A0%AC-%EC%98%88%EC%A0%9C---1)
- [삽입 정렬](https://github.com/genesis12345678/TIL/blob/main/algorithm/sorting/insertionSort/InsertionSort.md#%EC%82%BD%EC%9E%85-%EC%A0%95%EB%A0%AC) - `O(N^2)`
  - [예제 문제 - 1](https://github.com/genesis12345678/TIL/blob/main/algorithm/sorting/insertionSort/Example_1.md#%EC%82%BD%EC%9E%85-%EC%A0%95%EB%A0%AC-%EC%98%88%EC%A0%9C---1)
- [퀵 정렬](https://github.com/genesis12345678/TIL/blob/main/algorithm/sorting/quickSort/QuickSort.md#%ED%80%B5-%EC%A0%95%EB%A0%AC) - `pivot`, 평균 : `O(nlogn)`, 최악 : `O(n^2)`
  - [예제 문제 - 1](https://github.com/genesis12345678/TIL/blob/main/algorithm/sorting/quickSort/Example_1.md#%ED%80%B5-%EC%A0%95%EB%A0%AC-%EC%98%88%EC%A0%9C---1)
- [병합 정렬](https://github.com/genesis12345678/TIL/blob/main/algorithm/sorting/mergeSort/MergeSort.md#%EB%B3%91%ED%95%A9-%EC%A0%95%EB%A0%AC) - 분할 정복, `O(nlogn)`
  - [예제 문제 - 1](https://github.com/genesis12345678/TIL/blob/main/algorithm/sorting/mergeSort/Example_1.md#%EB%B3%91%ED%95%A9-%EC%A0%95%EB%A0%AC-%EC%98%88%EC%A0%9C---1)
  - [예제 문제 - 2](https://github.com/genesis12345678/TIL/blob/main/algorithm/sorting/mergeSort/Example_2.md#%EB%B6%84%ED%95%A0-%EC%A0%95%EB%B3%B5-%EC%98%88%EC%A0%9C---2)
- [기수 정렬](https://github.com/genesis12345678/TIL/blob/main/algorithm/sorting/radixSort/RadixSort.md#%EA%B8%B0%EC%88%98-%EC%A0%95%EB%A0%AC) - 계수 정렬(`counting sort`), `O(kn)`
  - [예제 문제 - 1](https://github.com/genesis12345678/TIL/blob/main/algorithm/sorting/radixSort/Example_1.md#%EA%B8%B0%EC%88%98-%EC%A0%95%EB%A0%AC-%EC%98%88%EC%A0%9C---1)

</details>



