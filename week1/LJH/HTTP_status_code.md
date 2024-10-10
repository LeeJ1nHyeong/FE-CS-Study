# HTTP Status Code

## 1XX - 정보 전달(Informational)
> 클라이언트의 요청에 대해 성공적으로 수신을 했고 서버에서 `처리중인 정보`를 알리는 코드

| Status Code | 상태 메세지         | 설명                     |
| ----------- | ------------------- | ------------------------ |
| 100         | Continue            | 계속 진행하라는 의미       |
| 101         | Switching protocols | 프로토콜 전환이 필요함     |
| 102         | Processing          | 처리 중                   |

<br/>

## 2XX - 성공(Success)
> 서버가 요청을 `성공`적으로 받았음을 알리는 코드

| Status Code | 상태 메세지        | 설명      |
| ----------- | ------------------ | --------- |
| 200         | OK                 | 서버가 요청을 성공적으로 처리했음을 의미 |
| 201         | Created            | 요청이 처리되어 새로운 리소스가 생성됨 |
| 202         | Accepted            | 요청은 접수했지만, 처리가 완료되지 않음 |
| 204         | No Content         | 처리를 성공했지만, 컨텐츠가 존재하지 않음 |

<br/>

## 3XX - 리다이렉션(Redirection)
> 요청 완료를 위해 `리다이렉션`이 필요하다는 것을 알리는 코드

| Status Code | 상태 메세지        | 설명     |
| ----------- | ------------------ | --------- |
| 301         | Moved Permanently | 지정한 리소스가 새로운 URI로 영구 이동 |
| 303         | See Other | 다른 위치로의 요청이 필요 |
| 307         | Temporary Redirect | 임시 리다이렉션 요청이 필요 |

<br/>

## 4XX - 클라이언트 요청 에러(Client Error)
> `클라이언트 측의 요청 에러`로 발생하는 코드

| Status Code | 상태 메세지        |설명     |
| ----------- | ------------------ |---------|
| 400         | Bad Request | 요청의 구문이 잘못됨 |
| 401         | Unauthorized | 요청자가 **인증**이 되지 않아 리소스에 접근할 수 없음 |
| 403         | Forbidden | 지정한 리소스에 대해 **접근 권한이 없음** |
| 404         | Not Found | 지정한 리소스을 찾을 수 없음     |
| 405         | Method Not Allowed | 요청한 메서드가 서버 측에서 허용하지 않음 |

<br/>

## 5XX - 서버 에러(Server Error)
> `서버 측의 에러`로 발생하는 코드

| Status Code | 상태 메세지        |설명     |
| ----------- | ------------------ |---------|
| 500         | Internal Server Error | 서버에 오류가 발생하여 작업을 수행할 수 없음을 알림 |
| 502         | Bad Gateway | 게이트웨이 문제로 잘못된 응답을 수신 |
| 503         | Service Unavailable | 서버가 요청 처리를 할 수 없는 상태(서비스 이용 불가) |
| 504         | Gateway Timeout | 게이트웨이 시간 초과 |

<br/>

---

### 예상 꼬리 질문
* 401(Unauthorized)과 403(Forbidden)의 차이점이 무엇인가요?
  
  401 에러는 요청자가 **인증**이 되지 않은 상태이며, 403 에러는 요청자가 인증은 됐지만 **접근 권한**이 없어 리소스에 접근할 수 없는 상태입니다.

<br/>

---

### 참고 자료
[HTTP 상태 코드 표 전체 요약 정리](https://hongong.hanbit.co.kr/http-%EC%83%81%ED%83%9C-%EC%BD%94%EB%93%9C-%ED%91%9C-1xx-5xx-%EC%A0%84%EC%B2%B4-%EC%9A%94%EC%95%BD-%EC%A0%95%EB%A6%AC/)

[HTTP 상태 코드(1XX ~ 5XX) 종류 총정리](https://inpa.tistory.com/entry/HTTP-%F0%9F%8C%90-%EC%83%81%ED%83%9C-%EC%BD%94%EB%93%9C-1XX-5XX-%EC%B4%9D%EC%A0%95%EB%A6%AC%ED%8C%90-%F0%9F%93%96)
