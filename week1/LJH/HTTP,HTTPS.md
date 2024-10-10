# HTTP, HTTPS

## HTTP (HyperText Transfer Protocol)
* 웹 서버와 클라이언트 간의 문서를 교환하기 위한 통신 규약
* 웹에서만 사용하는 프로토콜로 TCP/IP 기반으로 서버와 클라이언트 간의 요청과 응답을 전송한다.

### HTTP의 문제점
* `보안 취약성` : 데이터를 암호화하지 않고 평문으로 전송하기 때문에 개인 정보나 민감한 데이터가 노출될 우려가 있음
* `무결성 문제` : 데이터 전송 중에 변경되거나 조작될 가능성이 존재하여 정보의 정확성을 보장할 수 없음
* `신원 보증의 부재` : 서버의 신원을 확인하는 기능이 없어 제3자가 서버를 위장하여 클라이언트와 통신할 수 있기 때문에 사이버 공격 우려가 있음

<br/>

## HTTPS (HyperText Transfer Protocol Secure)
* HTTP의 문제점을 보완하기 위해 등장
* **기존 HTTP에서 보안이 강화된 버전**
* SSL/TLS 프로토콜을 사용하여 데이터의 암호화를 제공
* 메시지 다이제스트(Message Digest)를 사용하여 데이터의 변조 여부를 확인하면서 데이터의 무결성을 보장
* 인증 기관에 의해 발급된 서버 인증서를 사용하여 서버의 신원을 확인

<br/>

---

### 예상 꼬리 질문
* SSL과 TLS가 무엇인가요?

  SSL(Secure Sockets Layer)과 TLS(Transport Layer Security)은 네트워크 통신에서 데이터의 보안 및 기밀성을 제공하기 위한 프로토콜입니다. 브라우저는 이 인증서를 통해 진위 여부를 확인하고, 확인이 완료되면 보안 연결을 통해 전송된 모든 데이터가 암호화됩니다. SSL은 초기 버전이고, TLS는 SSL의 후속 버전이지만 일반적으로 "SSL/TLS"라는 용어로 함께 언급되거나 특별하게 구분하지 않고 SSL이라고 말하기도 합니다.

<br/>

---

### 참고 자료

[HTTP와 HTTPS의 차이는 무엇일까?](https://velog.io/@hyoribogo/what-is-the-defference-between-http-and-https)
