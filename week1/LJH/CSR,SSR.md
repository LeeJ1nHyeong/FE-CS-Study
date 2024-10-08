# CSR과 SSR

## CSR (Client Side Rendering)
* 클라이언트 측에서 렌더링을 진행하여 화면을 보여주는 방식
* 최초 로드 시에만 필요한 파일들을 전부 받은 상태에서 렌더링을 진행하고, 이 후에는 사용자의 인터렉션에 따라 필요한 부분에 대해서만 요청하여 새로 렌더링을 진행하는 방식입니다. 

### 장점
* 새로고침이 발생하지 않기 때문에 사용자 경험에 도움을 줌
* 초기 로딩 이후 빠른 웹사이트 렌더링 가능
* 필요한 부분만 새로 렌더링을 하기 때문에 트래픽 감소

### 단점
* 초기 로딩 속도가 느림
* SEO(검색 엔진 최적화)에 불리

<br/>

## SSR (Server Side Rendering)
* 서버 측에서 렌더링을 진행하여 화면을 보여주는 방식
* 사용자 요청이 들어올 때마다 서버 측에서 새로 HTML 파일을 만들어서 화면을 한꺼번에 제공하는 방식입니다.

### 장점
* SEO(검색 엔진 최적화)에 유리
* 초기 로딩 속도가 빠름

### 단점
* 서버에 요청할 때마다 새로고침을 해야함
* 초기 로딩 이후 페이지 이동 시 속도가 CSR보다 느림
* 서버 과부하

<br/>

---


### 예상 꼬리 질문
* SPA가 무엇인지 설명해주세요.

  Single Page Application의 약자로, 한 페이지 내에서 내용을 동적으로 변경하는 형태의 애플리케이션을 의미합니다.

* SEO가 무엇인지 설명해주세요.

  Search Engine Optimization의 약자로, 웹사이트가 유기적인 검색방식을 통해 검색 엔진에서 상위에 노출될 수 있도록 최적화하는 과정을 뜻합니다.

* SSR이 SEO에 유리한 이유가 무엇인가요?

  SSR을 통해 HTML이 완전히 로딩된 상태로 크롤러에 제공이 되기 때문에 크롤러가 더 많은 정보를 인식할 수 있으며, 그 결과로 더 높은 검색 결과 순위를 얻을 수 있기 때문입니다.

<br/>

---

### 참고 자료
[서버사이드렌더링 vs 클라이언트 사이드렌더링 (SSR과 CSR)](https://velog.io/@jhyun_k/%EC%84%9C%EB%B2%84%EC%82%AC%EC%9D%B4%EB%93%9C%EB%A0%8C%EB%8D%94%EB%A7%81-vs-%ED%81%B4%EB%9D%BC%EC%9D%B4%EC%96%B8%ED%8A%B8-%EC%82%AC%EC%9D%B4%EB%93%9C%EB%A0%8C%EB%8D%94%EB%A7%81-SSR%EA%B3%BC-CSR)

[이제는 알아야겠다! CSR과 SSR의 차이점과 장단점](https://dev-ellachoi.tistory.com/28)

[SSR 서버사이드렌더링의 원리와 SEO에 미치는 영향](https://www.next-t.co.kr/seo/seo%ED%8A%B8%EB%A0%8C%EB%93%9C/ssr-%EC%84%9C%EB%B2%84%EC%82%AC%EC%9D%B4%EB%93%9C%EB%A0%8C%EB%8D%94%EB%A7%81%EC%9D%98-%EC%9B%90%EB%A6%AC%EC%99%80-seo%EC%97%90-%EB%AF%B8%EC%B9%98%EB%8A%94-%EC%98%81%ED%96%A5/)

