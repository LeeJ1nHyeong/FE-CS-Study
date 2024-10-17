# 호이스팅 (Hoisting)

* Javascript에서 코드 실행 전 변수 선언과 함수 선언이 해당 스코프의 최상단으로 끌어올려지는 현상

## 변수 호이스팅

```javascript
console.log(x); // undefined
var x = 5;
console.log(x); // 5

console.log(y); // ReferenceError: y is not defined
let y = 5;
```

* `var` : 변수 선언과 초기화가 동시에 이루어지기 때문에 `undefined`로 초기화된 상태에서 호이스팅이 진행

* `let`, `const` : 변수 선언과 초기화가 분리되어 진행되면서 초기화되지 않은 상태로 호이스팅이 진행되기 때문에 `ReferenceError`가 발생

  * 스코프 시작 단계 ~ 초기화 이전의 구간 -> `TDZ (Temporal Dead Zone)`

<br/>

## 함수 호이스팅

```javascript
// 함수 선언문 : 호이스팅으로 정상 출력
console.log(sum(5, 3)); // 8
function sum(a, b) {
    return a + b;
}

// 함수 표현식 : 변수 호이스팅의 규칙을 따르기 때문에 TypeError 발생
console.log(multiply(5, 3)); // TypeError: multiply is not a function
var multiply = function(a, b) {
    return a * b;
};
```

* `함수 선언문` : 호이스팅으로 인해 어느 위치에서 함수를 실행해도 정상 작동

* `함수 표현식` : 변수 호이스팅 규칙을 따르기 때문에 표현식보다 앞선 위치에서 호출을 진행하면 TypeError 발생

<br/>

---

### 예상 꼬리 질문

* 호이스팅이 발생하는 이유가 무엇인가요?

  Javascript 엔진이 코드 실행 전에 변수 선언과 함수 선언을 미리 메모리에 저장하는 방식 때문에 발생합니다. 실행 전에 먼저 코드를 스캔하여 선언에 해당하는 부분을 찾아 메모리에 미리 저장을 한 뒤에 실행을 하기 때문에 호이스팅이 발생할 수 있습니다.

* 호이스팅을 아는 것이 중요한 이유가 무엇인가요?

  호이스팅에 대한 이해를 통해 코드 동작을 예측할 수 있고, 버그를 방지할 수 있습니다. 이를 통해 더 깔끔하고 효율적인 코드를 작성할 수 있습니다.

* 호이스팅을 피하는 방법이 있을까요?

  변수 선언을 최상단에서 진행하기, 변수 선언 시 var보다는 const와 let을 사용하는 것을 권장

<br/>

---

### 참고 자료

[호이스팅(Hoisting)이란?](https://hanamon.kr/javascript-%ED%98%B8%EC%9D%B4%EC%8A%A4%ED%8C%85%EC%9D%B4%EB%9E%80-hoisting/)

[자바스크립트의 호이스팅(Hoisting) 이해하기](https://f-lab.kr/insight/understanding-javascript-hoisting)
