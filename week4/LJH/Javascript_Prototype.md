# Javascript Prototype

Javascript에서 어떤 객체가 상속을 받기 위한 부모 역할을 담당하는 객체

## Prototype이 존재하는 이유

* Javascript에는 Class가 존재하지 않았었기 때문에 객체 지향 프로그래밍을 위해 상속을 받아야 할 부모 객체가 필요했고 Prototype이 그 역할을 맡게 됨
* 현재는 ES6에서 Class가 추가됨

## Prototype 구현

```javascript

function Person() {}  // 프로토타입 객체 Person

const lee = new Person();
const kim = new Person();

// getType 함수를 추가하여 "인간"을 return하는 함수 추가
Person.prototype.getType = function () {
    return "인간";
}

console.log(lee.getType());  // 인간
console.log(kim.getType());  // 인간

```

* `{프로토타입 객체}.prototype.{프로퍼티}` : 프로토타입 객체에 해당하는 객체 모두에게 프로퍼티 부여

## Prototype의 특징

### 프로토타입 체인(Chain)

객체의 프로퍼티나 메서드를 찾기 위해 자바스크립트 엔진은 먼저 해당 객체에서 직접 찾고, 없으면 프로토타입 체인(prototype chain)을 따라 올라가며 부모 객체의 프로퍼티를 찾습니다. 이 과정을 통해 객체는 프로토타입 체인을 통해 계층적으로 프로퍼티와 메서드를 상속받습니다.

### 프로토타입 객체

JavaScript의 모든 함수는 `prototype`이라는 기본 프로퍼티를 가지고 있으며, 이 프로퍼티는 새 객체를 생성할 때 상속의 기반이 됩니다. 예를 들어, 생성자 함수로 만든 객체는 이 `prototype` 객체를 통해 메서드나 프로퍼티를 상속받습니다.

### proto 프로퍼티

모든 객체는 `__proto__`라는 숨겨진 프로퍼티를 가지며, 이 프로퍼티는 해당 객체의 부모 프로토타입을 가리킵니다. 이 프로퍼티를 통해 객체는 자신의 부모 객체와 연결되고, 프로토타입 체인을 형성합니다.

<br/>

---

### 예상 꼬리 질문


<br/>

---

### 참고 자료

[Javascript: 프로토타입(prototype) 이해](https://www.nextree.co.kr/p7323/)

[프로토타입](https://poiemaweb.com/js-prototype)

