# HTTP Status Code

## 1XX - 정보 전달(Informational)
> 클라이언트의 요청에 대해 성공적으로 수신을 했고 서버에서 처리중인 정보를 알리는 코드

| Status Code | 상태 메세지        |설명     |
| ----------- | ------------------ |---------|
| 100         | Continue           |설명     |
| 101         | Switching protocols |설명     |

## 2XX - 성공(Success)
> 서버가 요청을 `성공`적으로 받았음을 알리는 코드

| Status Code | 상태 메세지        |설명     |
| ----------- | ------------------ |---------|
| 200         | OK |     |
| 201         | Created |     |
| 204         | No Content |     |

## 3XX - 리다이렉션(Redirection)
> 요청 완료를 위해 리다이렉션이 필요하다는 것을 알리는 코드

| Status Code | 상태 메세지        |설명     |
| ----------- | ------------------ |---------|
| 301         | Moved Permanently |설명     |

## 4XX - 클라이언트 요청 에러(Client Error)
> 클라이언트 측의 요청 에러로 발생하는 코드

| Status Code | 상태 메세지        |설명     |
| ----------- | ------------------ |---------|
| 400         | Bad Request           |설명     |
| 401         | Unauthorized |설명     |
| 403         | Forbidden |설명     |
| 404         | Not Found |설명     |
| 405         | Method Not Allowed |설명     |

## 5XX - 서버 에러(Server Error)
> 서버 측의 에러로 발생하는 코드

| Status Code | 상태 메세지        |설명     |
| ----------- | ------------------ |---------|
| 500         | Internal Server Error | 서버에 오류가 발생하여 작업을 수행할 수 없음을 알림 |
| 502         | Bad Gateway | 설명     |
| 503         | Service Unavailable | 서버가 요청 처리를 할 수 없는 상태 |
| 504         | Gateway Timeout | 설명     |

---

### 예상 꼬리 질문
* 200(OK)과 201(Created)의 차이점이 무엇인가요?

* 401(Unauthorized)과 403(Forbidden)의 차이점이 무엇인가요?

 
