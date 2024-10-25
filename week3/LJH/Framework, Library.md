# 프레임워크와 라이브러리

* **제어 흐름의 주도성**을 누가 갖고 있는지에 대해 차이가 있습니다.
* **프레임워크**는 프레임워크 자체가 스스로 흐름을 주도하여 개발자 코드를 가져와서 실행 -> 제어의 역전 (IoC)
* **라이브러리**는 개발자가 전체적인 흐름을 직접 만들고 제어

## 프레임워크 (Framework)

* 원하는 기능 구현에 집중하여 개발할 수 있도록 일정한 형태와 기능을 갖추고 있는 골격, 뼈대를 의미
* 애플리케이션 개발 시 필수적인 코드, 알고리즘, DB연동과 같은 기능을 위해 어느정도 구조(뼈대)를 제공하고, 이러한 구조위에서 사용자가 코드를 작성해서 애플리케이션을 개발
* 앱/서버 등의 구동, 메모리관리, 이벤트 루프 등 공통된 부분은 프레임워크가 관리하고, 사용자(개발자)는 프레임워크가 정해준 방식대로 클래스, 메소드를 구현

## 라이브러리 (Library)

* 단순 활용가능한 도구들의 집합
* 소프트웨어를 개발할 때 컴퓨터 프로그램이 사용하는 비휘발성 자원의 모임
* 특정 기능만을 제공할 뿐 어플리케이션의 전체 구조에는 관여하지 않음

<br/>

---

### 예상 꼬리 질문

* React를 라이브러리라고 하는 이유가 무엇인가요? (React는 프레임워크인가요, 라이브러리인가요?)

  프레임워크는 기능 구현에 집중하기 위한 뼈대역할을 하는 것이고, 라이브러리는 전체적인 틀이 아닌 기능을 제공하는 형태입니다. React는 웹 페이지 UI를 제작하는 `기능`을 제공하기 때문에 라이브러리입니다. 실제로 React 공식문서에서도 `라이브러리`라고 명시되어있습니다.

<br/>

---

### 참고 자료

[프레임워크(Framework)와 라이브러리(Library)의 차이](https://idkim97.github.io/2022-08-16-%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8C%ED%81%AC%20vs%20%EB%9D%BC%EC%9D%B4%EB%B8%8C%EB%9F%AC%EB%A6%AC/)

[프레임워크 vs 라이브러리](https://velog.io/@whitecloud94/%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8C%ED%81%AC-vs-%EB%9D%BC%EC%9D%B4%EB%B8%8C%EB%9F%AC%EB%A6%AC)