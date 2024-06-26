# GET 요청과 POST 요청의 차이는 무엇인가요?

- **GET**과 **POST** 요청 둘 다 클라이언트가 서버에 요청하기 위한 HTTP 메서드이지만 차이가 있다.
- **[GET]**
  - 주로 리소스를 조회할 때 사용(`SELECT`)
  - 서버에 전달하고 싶은 데이터를 쿼리 스트링(쿼리 파라미터)을 통해서 전달, 메시지 바디가 없다.
  - 캐시(`Cache`)가 가능하며, `cache-control` 헤더를 통해 캐시 옵션을 지정할 수 있다.
  - GET 요청은 길이 제한이 있으며, 브라우저 히스토리에 남는다.
- **[POST]**
  - 주로 리소스를 등록(생성)할 때 사용(`INSERT`)
  - 서버에 전달하고 싶은 데이터를 메시지 바디에 담아서 전달하기 때문에 대용량 데이터를 전송할 수 있다.
  - 캐시(`Cache`)되지 않는다.
  - POST 요청은 데이터 길이에 제한이 없고, 브라우저 히스토리에 남지 않는다.
  - POST 요청은 요청 헤더의 `Content-Type`에 요청 데이터의 타입을 표시해야 한다.

### GET과 POST 차이 정리

- **목적**
  - `GET`은 리소스를 조회할 때, `POST`는 리소스를 등록할 때 사용
- **메시지 바디 유무**
  - `GET`은 쿼리 파라미터를 통해 데이터를 전달하기 때문에 메시지 바디가 없다.
  - `POST`는 메시지 바디에 데이터를 담아서 전달한다.
- **멱등성**
  - `GET`은 멱등하다, `POST`는 멱등하지 않다.
  - 멱등성은 여러 번 요청해도 결과가 달라지지 않는 성질이다.
  - `GET` 요청은 단순 조회이기 때문에 여러 번 요청해도 응답이 같지만, `POST`는 리소스를 새로 생성하기 때문에 멱등이 아니다.
  - 멱등하다를 판단할 수 있는 근거는 예를 들어 서버에 장애가 있어 정상 응답을 주지 못했을 때, 클라이언트가 모르고 같은 요청을 다시 해도 되는가에 있다.