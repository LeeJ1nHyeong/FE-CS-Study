# Promise, async/await

**Promise**와 **async/await**는 Javascript에서 비동기 처리를 위한 방법입니다.

## Promise

* 비동기 작업의 최종 완료 또는 실패를 나타내는 객체
* `.then()` 메서드를 통해 비동기 작업이 성공했을 때의 로직을 실행
* `.catch()` 메서드를 통해 비동기 작업이 실패했을 때의 로직을 실행
* 여러 개의 `.then()`을 사용하여 비동기 작업을 순차적으로 처리할 수 있지만, 양이 많을 경우 **콜백 지옥**이 생길 우려가 있음

## async/await

* 비동기 코드를 동기 코드처럼 작성 가능
* 함수에 `async` 키워드를 붙이고, 해당 함수 내의 비동기 처리 대상에 `await` 키워드를 붙여 비동기 처리가 끝날 때까지 대기
* try-catch문을 활용하여 에러처리를 하기 때문에 가독성이 높아지고, 에러를 쉽게 잡을 수 있는 장점을 갖고 있음

<br/>

---

### 예상 꼬리 질문



<br/>

---

### 참고 자료

[8. Async/Await와 Promise의 차이에 대해 설명해주세요.](https://velog.io/@p_seo_hn/8.-AsyncAwait%EC%99%80-Promise%EC%9D%98-%EC%B0%A8%EC%9D%B4%EC%97%90-%EB%8C%80%ED%95%B4-%EC%84%A4%EB%AA%85%ED%95%B4%EC%A3%BC%EC%84%B8%EC%9A%94)
