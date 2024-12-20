# TCP, UDP

## TCP (Transmission Control Protocol, 전송 제어 프로토콜)

* 인터넷상에서 데이터를 메세지의 형태로 보내기 위해 IP와 함께 사용하는 프로토콜
* `연결 지향 방식`으로 `패킷 교환 방식`을 사용
* `3-way handshake` 과정을 통해 연결을 설정하고 `4-way handshake` 과정을 통해 해제
* 높은 신뢰성을 보장하지만 UDP보다 느림 -> 신뢰성 있는 전송이 중요할 때(파일 전송 등)에 사용 

## UDP (User Datagram Protocol, 데이터그램 프로토콜)

* 데이터를 데이터그램 단위로 처리하는 프로토콜
  * `데이터그램` : 독립적인 관계를 지니는 패킷
* `비연결형 프로토콜`로 연결을 위해 할당되는 논리적인 경로가 존재하지 않음 -> 각의 패킷은 다른 경로로 전송되고, 각각의 패킷은 독립적인 관계를 가지면서 다른 경로로 독립적으로 처리
* TCP보다 속도가 빠르지만 신뢰성이 낮음 -> 연속성이 중요한 서비스(스트리밍 서비스 등)에 자주 사용

<br/>

---

### 예상 꼬리 질문

<br/>

---

### 참고 자료

[TCP와 UDP의 특징과 차이](https://mangkyu.tistory.com/15)
