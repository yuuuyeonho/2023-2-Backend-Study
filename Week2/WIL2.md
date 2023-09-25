### 과제1
## HTTP란?
서로 다른 시스템들 사이에서 통신을 주고 받게 해주는 application 계층의  protocol

#### 특징
o Transfer layer - Tcp
o 비 연결성
o 무상태성

1. TCP연결을 열어준다.
2. HTTP메시지를 전송한다.
3. 서버가 보낸 응답을 읽는다.
4. 연결을 닫거나 다른 요청을 위해 재사용한다.

HTTP는 HTTP message를 통해 데이터를 주고받는다.
request(요청), response(응답)

http method, 경로, http 버전, 헤더

http method - 주로 GET, POST, PUT, PATCH, DELETE 사용


<br/>

### 과제2
HTTPS는?\
HTTP에 데이터 암호화가 추가된 프로토콜  
<br/>

### 과제3
이벤트 목록 조회  
/events/lists  

이벤트 조회  
/events/1

이벤트 등록  
/events/new

이벤트 수정  
/events/modify

이벤트 삭제  
/events/remove

이벤트 상태 변경  
/events/state

특정 이벤트의 주문 목록 조회  
/events/1/order-lists

멤버 목록 조회
/members/lists

특정 멤버 권한 변경  
/members/1/right

특정 멤버 정보 조회  
/members/1/user-info

특정 멤버 정보 변경  
/members/1/user_info/modify

멤버 등록  
/member/new

<br/><br/>

---
내용 정리

## HTTP란?
서로 다른 시스템들 사이에서 통신을 주고 받게 해주는 application 계층의  protocol

#### 특징
o Transfer layer - Tcp
o 비 연결성
o 무상태성

1. TCP연결을 열어준다.
2. HTTP메시지를 전송한다.
3. 서버가 보낸 응답을 읽는다.
4. 연결을 닫거나 다른 요청을 위해 재사용한다.

HTTP는 HTTP message를 통해 데이터를 주고받는다.
request(요청), response(응답)

http method, 경로, http 버전, 헤더

http method - 주로 GET, POST, PUT, PATCH, DELETE 사용



## REST

자원을 이름으로 구분하여 해당 자원의 상태를 주고, 받는 모든 것을 말한다.
핵심 3요소 - 자원, 조작, 표현

자원: 서버에 있는 것, 데이터 혹은 이미지 하나하나를 의미, URI를 통해 자원을 명시하고 구분
조작: Client는 HTTP method를 이용하여 자원에 대한 조작을 요청
표현: Client가 Server에게 자원에 대한 조작을 요청하면 Server는 이에 대한 적절한 응답(representation)을 보냄

#### REST원칙
인터페이스 일관성
무상태성
Resource 지향 아키텍쳐
클라이언트-서버 아키텍쳐
캐시 기능
계층화
자체 표현 구조

## RESTful API 디자인 가이드
1. URI의 리소스명은 소문자를 사용한다.
2. 자원에 대한 행위는 HTTP 메서드를 통해서 표현하자
3. 하이픈은 URI의 가독성을 위해서 사용, 밑줄은 사용하지 않는다.
4. 슬래시 구분자는 계층 관계를 나타낼 때 사용하며 URI의 마지막 문자로 사용하면 안된다.
5. 파일 확장자는 URI에 포함시키지 않는다.

## 웹 어플리케이션
정적 페이지(Static Pages) / 동적 페이지(Dynamic Pages)

#### WAS
HTTP를 통해 애플리케이션을 수행해주는 미들웨어(소프트웨어)
주요기능
1.  프로그램 실행 환경 및 DB접속 기능 제공
2. 여러 트랜잭션 관리 기능
3. 업무 처리하는 비즈니스 로직 수행  
<br/><br/><br/>

---
#### 오늘의 후기  
평소에 많이 들어본 단어들인데도 어렵다...  
그리고 URI설계하는거 너무너무 생각이 안난다.