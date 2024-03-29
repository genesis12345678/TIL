# 액츄에이터

## 프로덕션 준비 기능이란?

개발자가 애플리케이션을 개발할 때 기능 요구사항만 개발하는 것은 아니다. <br>
개발자는 서비스에 문제가 없는지 모니터링하고 지표들을 심어서 감시해야 하는 또 다른 중요한 업무가 있다.

운영 환경에서 서비스할 때 필요한 이런 기능들을 **프로덕션 준비 기능**이라 한다. 프로덕션을 운영에 배포할 때 준비해야 하는 비 기능적 요소들을 뜻한다.
- 지표(metric), 추적(tarce), 감사(auditing)
- 모니터링

애플리케이션이 현재 살아있는지, 로그 정보는 정상적으로 설정 되었는지, 커넥션 풀은 얼마나 사용되고 있는지 등을 확인할 수 있어야 한다.

스프링 부트가 제공하는 `액츄에이터`는 이런 프로덕션 준비 기능을 매우 편리하게 사용할 수 있는 다양한 편의 기능들을 제공한다.<br>
더 나아가 마이크로미터, 프로메테우스, 그라파나 같은 모니터링 시스템과 매우 쉽게 연동할 수 있는 기능도 제공한다.

- [액츄에이터 시작](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/actuator/Basic.md)
  - [엔드포인트 설정](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/actuator/Basic.md#%EC%97%94%EB%93%9C%ED%8F%AC%EC%9D%B8%ED%8A%B8-%EC%84%A4%EC%A0%95)
  - [다양한 엔드포인트](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/actuator/Basic.md#%EB%8B%A4%EC%96%91%ED%95%9C-%EC%97%94%EB%93%9C%ED%8F%AC%EC%9D%B8%ED%8A%B8)
- [헬스 정보](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/actuator/Health.md)
- [애플리케이션 정보](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/actuator/Info.md)
- [로거](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/actuator/Logger.md)
- [HTTP 요청 응답 기록](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/actuator/HttpExchange.md)
- [액츄에이터 보안](https://github.com/genesis12345678/TIL/blob/main/Spring/springboot/actuator/Security.md)