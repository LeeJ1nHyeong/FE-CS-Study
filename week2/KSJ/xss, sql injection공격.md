# XXS, sql injection공격 이란?


## XSS
    XSS는 웹 애플리케이션의 취약점을 이용해 악성 스크립트를 웹 페이지에 삽입하는 공격 방식입니다. 공격자가 악성 코드를 삽입하면, 해당 웹 페이지를 방문한 사용자의 브라우저가 이를 실행하게 되어 사용자의 세션 쿠키 탈취, 사이트 변조, 악성 코드 실행 등이 발생할 수 있습니다. XSS는 주로 사용자가 입력한 데이터를 필터링 없이 출력할 때 발생합니다.
## SQL Injection
    SQL Injection은 웹 애플리케이션의 입력 필드를 통해 악성 SQL 쿼리를 삽입해 데이터베이스를 공격하는 기법입니다. 공격자가 데이터베이스에 직접적인 명령을 실행하여 데이터를 탈취하거나, 삭제, 수정하는 등의 피해를 유발할 수 있습니다. SQL Injection은 주로 웹 애플리케이션에서 사용자의 입력을 제대로 필터링하지 않을 때 발생합니다.
---



### 참고 자료
* https://velog.io/@layl__a/%ED%98%BC%EA%B3%B5-XSS-%EB%9E%80-%EB%AC%B4%EC%97%87%EC%9D%B8%EC%A7%80-%EC%98%88%EC%8B%9C%EB%A1%9C-%EC%82%B4%ED%8E%B4%EB%B3%B4%EC%9E%90
* https://www.cloudflare.com/ko-kr/learning/security/threats/sql-injection/