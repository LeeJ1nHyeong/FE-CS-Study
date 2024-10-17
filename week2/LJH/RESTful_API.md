# RESTful API

## REST (REpresentational State Transfer)

* 자원을 이름(자원의 표현)으로 구분하여 해당 자원의 상태(정보)를 주고 받는 모든 것을 의미
* 웹의 장점을 최대한 활용할 수 있는 아키텍처 스타일
* 클라이언트-서버 간의 통신 방식
* CRUD 연산을 수행하기 위해 URI로 메서드를 사용하여 요청 -> 요청을 위한 자원을 특정한 형태로 표현

### REST의 구성 요소

* 자원(Resource) : URI
* 행위(Verb) : HTML Method
* 자원의 표현(Representation of Source) : Json, Xml 등

### REST의 특징

* `서버-클라이언트 구조` : 자원이 있는 쪽이 서버, 자원을 요청하는 쪽이 클라이언트
* `무상태(Stateless)` : 각각의 요청을 독립적으로 처리
* `캐시 처리 가능` : 대량의 요청을 효율적으로 처리할 수 있습니다.
* `계층 구조`
* `인터페이스 일관성` : URI로 지정한 Resource에 대한 요청을 통일되고, 한정적으로 수행하는 아키텍처 스타일
* `자체 표현` : 요청 메시지만 보고도 쉽게 이해할 수 있는 자체 표현 구조

<br/>

## REST API

* REST의 특징을 기반으로 API를 구현한 것
* URI는 정보의 자원만 표현해야 하며, 자원의 행위는 HTTP Method에 명시
* 각 요청이 어떤 동작이나 정보를 위한 것인지를 그 요청의 모습 자체로 추론이 가능

### REST API의 규칙

* URI는 정보의 자원을 표현
* URI에 Method 포함 금지 (GET, POST, DELETE, UPDATE 등)
* URI에 명사 사용
* 슬래쉬(/)로 계층 관계 표현
* 이름이 길면 하이픈(-)을 사용
* 소문자로 구성
* 확장자 포함 금지
* HTTP 상태 코드를 사용

<br/>

## RESTful API

* 'REST API'를 제공하는 웹 서비스를 'RESTful' 하다고 할 수 있다.
* RESTful은 REST를 REST 답게 쓰기 위한 방법으로, 누군가가 공식적으로 발표한 것은 아니다.
* REST API의 설계 규칙을 올바르게 지킨 시스템을 RESTful하다고 함
* **RESTful하게 만든 API는 요청을 보내는 주소만으로도 어떤 것을 요청 하는지 파악이 가능**


<br/>

---

### 예상 꼬리 질문


<br/>

---

### 참고 자료

[REST, REST API, RESTful 특징](https://hahahoho5915.tistory.com/54)

[RESTful API 이란](https://velog.io/@somday/RESTful-API-%EC%9D%B4%EB%9E%80)

[REST란? REST API 와 RESTful API의 차이점](https://dev-coco.tistory.com/97)
