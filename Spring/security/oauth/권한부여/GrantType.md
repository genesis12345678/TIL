# OAuth 2.0 권한 부여 유형 - OAuth 2.0 Grant Type

---

## 권한 부여 유형

- 권한 부여란 클라이언트가 사용자를 대신해서 사용자의 승인 하에 인가 서버로부터 권한을 부여받는 것을 의미한다.
- OAuth 2.0 메커니즘은 다음과 같은 권한 부여 유형들을 지원하고 있으며 일부는 `Deprecated` 되었다.

### 1. Authorization Code Grant Type
   - 권한 코드 부여 타입
   - 서버 사이드 애플리케이션(웹 애플리케이션)
   - 보안에 가장 안전한 유형
### 2. Implicit Grant Type(Deprecated)
   - 암시적 부여 타입
   - 공개 클라이언트 애플리케이션(SPA 기반 자바스크립트 앱, 모바일 앱)
   - 보안에 취약
### 3. Resource Owner Password Credentials Grant Type(Deprecated)
   - 리소스 사용자 비밀번호 자격증명 부여 타입
   - 서버 애플리케이션
   - 보안에 취약
### 4. Client Credentials Grant Type
   - 클라이언트 자격 증명 권한 부여 타입
   - UI 또는 화면이 없는 서버 애플리케이션
### 5. Refresh Token Grant Type
   - 새로고침 토큰 부여 타입
   - 1번, 3번 유형에서 지원 된다.
### 6. PKCE-enhanced Authorization Code Grant Type
   - PKCE 권한 코드 부여 타입
   - 서버 사이드 애플리케이션, 공개 클라이언트 애플리케이션

---

## 매개 변수 용어

### 1. client_id
- 인가 서버에 등록된 클라이언트에 대해 생성된 고유 키

### 2. client_secret
- 인가 서버에 등록된 특정 클라이언트의 `client_id`에 대해 생성된 비밀 값 

### 3. response_type
클라이언트가 제공받길 원하는 응답 타입
- 애플리케이션이 권한 부여 코드 흐름을 시작하고 있음을 인증 서버에 알려준다.
- `code`, `token`, `id_token`이 있으며 `token`, `id_token`은 **implicit** 권한 부여 유형에서 지원해야 한다.
- 서버가 쿼리 문자열에 인증 코드(code), 토큰(token, id_token) 등을 반환

### 4. grant_type
- 권한 부여 타입 지정
- `authorization_code`, `password`, `client_credentials`, `refresh_token` 등

### 5. redirect_uri
로그인 성공 시 이동해야 하는 URI
- 사용자가 응용 프로그램을 성공적으로 승인하면 권한 부여 서버가 사용자를 다시 응용 프로그램으로 리다이렉트 한다.
- `redirect_uri`가 초기 권한 부여 요청에 포함된 경우 서비스는 토큰 요청에서도 이를 요구해야 한다.
- 토큰 요청의 `redirect_uri`는 인증 코드를 생성할 때 사용된 `redirect_uri`와 정확히 일치해야 한다. 그렇지 않으면 서비스는 요청을 거부해야 한다.

### 6. scope
제공받고자 하는 리소스 오너의 정보 목록
- 애플리케이션이 사용자 데이터에 접근하는 것을 제한하기 위해 사용된다.(email, profile, read, write 등)
- 사용자에 의해 특정 스코프로 제한된 권한 인가권을 발행함으로써 데이터 접근을 제한한다.

### 7. state
- 응용 프로그램은 임의의 문자열을 생성하고 요청에 포함하고 사용자가 앱을 승인한 후 서버로부터 동일한 값이 반환되는지 확인해야 한다.
- 이것은[ CSRF 공격](https://github.com/genesis12345678/TIL/blob/main/Spring/security/security/Cors_Csrf/Csrf.md)을 방지하는 데 사용된다.

---

[메인 ⏫](https://github.com/genesis12345678/TIL/blob/main/Spring/security/oauth/main.md)

[다음 ↪️ - OAuth 2.0 권한부여 유형 - 권한 부여 코드 승인 방식](https://github.com/genesis12345678/TIL/blob/main/Spring/security/oauth/%EA%B6%8C%ED%95%9C%EB%B6%80%EC%97%AC/Authorization.md)