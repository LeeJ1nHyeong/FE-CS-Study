# JWT (JSON Web Token)

* 웹에서 사용되는 JSON 형식의 토큰에 대한 표준 규격
* 주로 사용자의 인증(authentication) 또는 인가(authorization) 정보를 서버와 클라이언트 간에 안전하게 주고 받기 위해서 사용

## JWT의 구조

* `헤더(Header)` : 토큰 타입, 암호화 알고리즘 명시
* `페이로드(Payload)` : JWT에 넣을 데이터, JWT 발급 / 만료일 등 명시
* `서명(Signiture)` : 헤더와 페이로드가 비밀키로 서명되어 저장. 헤더와 페이로드의 변조 여부를 확인하는 역할

## JWT를 사용하는 이유

* 사용자 인증에 필요한 정보를 토큰 자체에 넣어두기 때문에 세션과 같이 별도와 저장관리소가 필요없음
* 쿠키로 전달하지 않아도 되기 때문에 쿠키를 사용함으로써 발생하는 취약점도 보완 가능

## AccessToken과 RefreshToken

* `AccessToken` : 서버 API를 직접 요청할 때 사용하는 토큰
* `RefreshToken` : AccessToken이 만료되었을 때 재발급을 하기 위한 목적으로 사용되는 토큰

<br/>

---

### 예상 꼬리 질문

* AccessToken을 단독으로 사용하지 않고 RefreshToken을 같이 사용하는 이유가 무엇인가요?

  두 토큰을 같이 사용하는 것은 AccessToken이 탈취될 경우를 대비하는 것입니다. AccessToken이 만료되거나 탈취를 당했을 경우 클라이언트가 RefreshToken을 이용하여 AccessToken을 재발급 요청하여 새로 발급받을 수 있습니다. 다만 RefreshToken도 탈취를 당할 위험이 있기 때문에 안전하게 저장하는 방법을 고려해야합니다.

<br/>

---

### 참고 자료

[우리는 왜 JWT를 사용하는가? / JWT 사용 이유](https://puleugo.tistory.com/138)

[JWT - Json Web Token](https://www.daleseo.com/jwt/)
