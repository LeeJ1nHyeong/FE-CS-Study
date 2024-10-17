# 이벤트 루프 (Event Loop)

브라우저 내부의 Call Stack, Callback Queue, Web API 등의 요소를 모니터링하여 비동기적으로 실행하는 작업을 관리하고 순차적으로 처리하여 프로그램의 실행 흐름을 관리하는 역할

## 동작 방식

1. `Call Stack 확인` : 현재 Call Stack이 비어 있는지 확인합니다. 만약 Call Stack에 아직 처리되지 않은 함수가 있다면 해당 함수가 완전히 실행될 때까지 기다립니다.
2. `Callback Queue 확인` : Call Stack이 비어있다면 Callback Queue를 확인합니다. Callback Queue에는 Web API에서 생성된 콜백 함수가 대기중입니다.
3. `함수 이동` : Callback Queue에서 가장 오래된 함수를 꺼내서 콜 스택으로 옮깁니다.
4. `함수 실행` : 해당 함수가 Call Stack에서 실행되고 실행이 끝나면 Call Stack에서 빠져나가게 됩니다.
5. 프로그램이 종료될 때까지 위 과정을 반복합니다.

<br/>

---

### 예상 꼬리 질문


<br/>

---

### 참고 자료

[이벤트 루프(Event Loop)에 대해서 파헤쳐 봅시다.](https://yong-nyong.tistory.com/71)
