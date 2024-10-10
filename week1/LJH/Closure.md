# Closure
* 함수와 그 함수가 선언됐을 때의 렉시컬 환경(Lexical environment)과의 조합
* 함수의 생명 주기가 종료되더라도 함수의 반환 값이 변수에 의해 아직 참조되고 있다면 렉시컬 환경에 남아 참조가 가능함
* 자신을 포함하고 있는 외부함수보다 내부함수가 더 오래 유지되는 경우, 외부 함수 밖에서 내부함수가 호출되더라도 외부함수의 지역 변수에 접근할 수 있는 형태의 함수

``` javascript
function outerFunc() {
  var x = 10;
  var innerFunc = function () { console.log(x); };
  return innerFunc;
}

/**
 *  함수 outerFunc를 호출하면 내부 함수 innerFunc가 반환된다.
 *  그리고 함수 outerFunc의 실행 컨텍스트는 소멸한다.
 */

var inner = outerFunc();
inner(); // 10
```
* 함수 `outerFunc`로 내부에 있는 함수 `innerFunc`을 호출하면서 `outerFunc`는 종료됨
* 하지만 `outerFunc`의 return 값인 `innerFunc`이 `inner`에 할당되면서 `outerFunc`의 지역변수인 `x`가 `innerFunc`에 의해 호출됨

<br/>

---

### 예상 꼬리 질문

<br/>

---

### 참고 자료
[1. 클로저(closure)의 개념](https://poiemaweb.com/js-closure)
