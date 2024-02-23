# 액츄에이터 시작

액츄에이터가 제공하는 프로덕션 준비 기능을 사용하려면 스프링 부트 액츄에이터 라이브러리를 추가해야 한다.

```groovy
implementation 'org.springframework.boot:spring-boot-starter-actuator'
```

`localhost:8080/actuator` 실행
```json
{
  "_links": { 
    "self": {
      "href": "http://localhost:8080/actuator", 
      "templated": false
    },
    "health-path": {
      "href": "http://localhost:8080/actuator/health/{*path}", 
      "templated": true
    },
    "health": {
      "href": "http://localhost:8080/actuator/health", 
      "templated": false
    } 
  } 
}
```
- 액츄에이터는 `/actuator` 경로를 통해서 기능을 제공한다.
- 화면에 보이는 `health`결과를 제공하는 URL을 실행해보자.
  - `localhost:8080/actuator/health` 실행
  - 결과 : `{"status": "UP"}`
  - 이 기능은 현재 서버가 잘 동작하고 있는지 애플리케이션의 헬스 상태를 나타낸다.

액츄에이터는 헬스 상태 외에 수 많은 기능을 제공하는데 이런 기능이 웹 환경에서 보이도록 노출해야 한다.

- `application.yml` 추가
```yaml
management:
  endpoints:
    web:
      exposure:
        include: "*"
```

이렇게 설정한 이후 다시 `localhost:8080/actuator`를 실행해 보면 액츄에이터가 제공하는 수 많은 기능을 볼 수 있다.

액츄에이터가 제공하는 기능 하나하나를 엔드포인트라 한다. 각각의 엔드포인트는 `/actuator/{엔드포인트명}` 형식으로 접근할 수 있다.

## 엔드포인트 설정

엔드포인트를 사용하려면 2가지 과정이 모두 필요하다.
- 엔드포인트 활성화
- 엔드포인트 노출

엔드포인트를 활성화 한다는 것은 해당 기능 자체를 사용할지 안할지 `on`, `off`를 선택하는 것이다.<br>
엔드포인트를 노출하는 것은 활성화된 엔드포인트를 HTTP에 노출할지, 아니면 JMX에 노출할지 선택하는 것이다.

**엔드포인트는 대부분 기본으로 활성화 되어 있다.**(`shutdown` 제외) 노출이 되어 있지 않을 뿐이다.<br>
따라서 어떤 엔드포인트를 노출할지 선택하면 된다.

**모든 엔드포인트를 웹에 노출**
```yaml
management:
  endpoints:
    web:
      exposure:
        include: "*"
```
- `*` 옵션은 모든 엔드포인트를 웹에 노출하는 것이다.(`shutdown` 엔드포인트는 기본으로 활성화 되지 않기 때문에 노출도 되지 않는다.)
- **엔드포인트 활성화 + 엔드포인트 노출이 둘다 적용되어야 사용할 수 있다.**

**엔드포인트 활성화**
```yaml
management: 
  endpoint:
    shutdown:
      enabled: true 
  endpoints:
    web:
      exposure: 
        include: "*"
```
- 특정 엔드포인트를 활성화 하려면 `management.endpoint.{엔드포인트명}.enabled=true`를 적용하면 된다.
- 이제 `localhost:8080/actuator/shutdown`을 `POST`로 호출해보면 서버가 종료된다.

**엔드포인트 노출**

스프링 공식 매뉴얼 예제
```yaml
management: 
  endpoints:
    jmx:
      exposure:
        include: "health,info"
```
- `jmx`에 `health, info`를 노출한다.

```yaml
management:
  endpoints:
    web:
      exposure:
        include: "*" 
        exclude: "env,beans"
```
- `web`에 모든 엔드포인트를 노출하지만 `env`, `beans`는 제외한다.

## 다양한 엔드포인트

각각의 엔드포인트를 통해서 개발자는 애플리케이션 내부의 수 많은 기능을 관리하고 모니터링 할 수 있다.

**자주 사용하는 엔드포인트 목록**
- `beans` : 스프링 컨테이너에 등록된 스프링 빈을 보여준다.
- `conditions` : `condition`을 통해서 빈을 등록할 때 평가 조건과 일치하거나 일치하지 않은 이유를 표시한다.
- `configprops` : `@ConfigurationProperties`를 보여준다.
- `env` : `Environment` 정보를 보여준다.
- `health` : 애플리케이션 헬스 정보를 보여준다.
- `httpexchanges` : HTTP 호출 응답 정보를 보여준다. `HttpExchangeRepository`를 구현한 빈을 별도로 등록해야 한다.
- `info` : 애플리케이션 정보를 보여준다.
- `loggers` : 애플리케이션 로거 설정을 보여주고 변경도 할 수 있다.
- `metrics` : 애플리케이션의 메트릭 정보를 보여준다.
- `mappings` : `@RequestMapping` 정보를 보여준다.
- `threaddump` : 쓰레드 덤프를 실행해서 보여준다.
- `shutdown` : 애플리케이션을 종료한다. 기본으로 비활성화 되어있다.

[전체 엔드포인트 공식 매뉴얼](https://docs.spring.io/spring-boot/docs/current/reference/html/actuator.html#actuator.endpoints)