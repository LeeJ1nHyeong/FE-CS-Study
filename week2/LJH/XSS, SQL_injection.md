# XSS, SQL Injection

## XSS (Cross Site Scripting)

* 권한 없는 사용자가 웹 사이트에 악의적인 스크립트를 삽입하여 공격하는 기법

### 공격 방법

* `Reflected XSS` : 사용자의 브라우저가 서버로부터 정상 HTML을 받고 URL에 포함된 공격 스크립트를 문자열로 추출해 함께 실행하는 과정에서 공격 스크립트가 실행
* `Stored XSS` : 웹 사이트의 게시판에 공격 스크립트를 포함한 게시글을 업로드하여 게시글을 접속한 사용자의 정보 탈취
* `DOM XSS` : 서버가 URL 파라미터를 검증없이 응답 HTML에 담고 사용자의 브라우저는 응답받은 비정상 HTML을 실행하는 과정에서 공격 스크립트가 실행

## SQL Injection

* 악의적으로 임의의 SQL문을 주입하여 데이터베이스가 비정상적으로 동작하도록 조작하는 행위

### 공격 방법

```sql
-- 정상
SELECT * FROM USER WHERE id = 'id' AND password = 'password'

-- SQL Injection
SELECT * FROM USER WHERE id = '' OR 1=1 -- ' AND password = 'password'
```

id 입력칸에 `' OR 1=1 -- `를 입력하여 WHERE 절에 있는 싱글쿼터를 닫아주기 위한 싱글쿼터와 OR 1=1 라는 구문을 이용해 WHERE 절을 모두 참으로 만들고, -- 를 넣어줌으로 뒤의 구문을 모두 주석 처리
-> USER 테이블 내의 모든 정보를 조회하여 탈취

<br/>

---

### 예상 꼬리 질문

* XSS를 예방하는 방법에는 어떤 것이 있을까요?
  
  * **입력값에 대한 검증 강화**
  * **Prepared Statement** : 특수문자를 자동으로 escaping 해줌
  * **Error Message 노출 금지** : 에러 메세지를 통해 쿼리문을 노출 시킬 우려가 있음
  * **웹 방화벽**
 
* SQL Injection을 예방하는 방법에는 어떤 것이 있을까요?

  * **문자열 Escape 처리**
  * **쿠키 보안옵션 (HttpOnly) 설정**
  * **웹 방화벽**
 
<br/>

---

### 참고 자료

[SQL Injection과 XSS (Cross-Site Scripting)](https://way-code.tistory.com/entry/SQL-Injection%EA%B3%BC-XSS-Cross-Site-Scripting)

[SQL Injection 이란? (SQL 삽입 공격)](https://noirstar.tistory.com/264)
