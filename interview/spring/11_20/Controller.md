# 어떻게 하나의 컨트롤러로 요청을 받을 수 있을까요?

- 컨트롤러는 컴포넌트 스캔의 대상이므로 스프링 컨테이너에 빈으로 등록된다.
- 빈은 싱글톤으로 관리되기 때문에 여러 쓰레드의 요청이 들어와도 하나의 컨트롤러 객체를 공유하면서 처리한다.
- 여러 쓰레드가 메서드에 대해 공유 자원으로써 접근해 사용하는 것이다.
- **싱글톤 패턴**이므로 `Thread-Safe` 하지 않아 공유 필드에 주의해야 하고, 상태를 유지하게 설계하면 안 된다.(`stateless`)