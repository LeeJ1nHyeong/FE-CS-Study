# CORS

`Cross-Origin Resource Sharing`의 약자로 서버 측에서 헤더를 통해서 다른 출처(웹)에서 자원에 접근할 수 있는 권한을 부여하도록 브라우저에게 알려주는 정책입니다. 예를 들어 웹 사이트 A가 API 서버 B에서 데이터를 가져오려 할 때, API 서버 B에서 CORS 허용 설정이 되어 있지 않으면 웹 브라우저에서 API 접근이 거부될 수 있습니다.


<br/>

---

### 예상 꼬리 질문

* CORS 에러가 발생했을 때의 대처방법이 무엇인가요?

  * `Access-Control-Allow-Origin 세팅하기` : 서버에서 Access-Control-Allow-Origin 헤더에 접근을 허용할 출처 도메인을 추가하거나 와일드카드 '*'로 세팅을 하여 모든 출처에서 접근을 허용할 수 있게 설정
  * `프록시 서버 사용` : 웹 애플리케이션이 리소스를 직접적으로 요청하는 대신, 프록시 서버를 사용하여 웹 애플리케이션에서 리소스로의 요청을 전달

<br/>

---

### 참고 자료

[CORS란 무엇인가?](https://velog.io/@effirin/CORS%EB%9E%80-%EB%AC%B4%EC%97%87%EC%9D%B8%EA%B0%80#cors%EC%9D%98-%EB%93%B1%EC%9E%A5-%EB%B0%B0%EA%B2%BD)
