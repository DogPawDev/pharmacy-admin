# pharmacy-admin
 
## 미리보기

- 바코드 입력
<img alt="barcode" src="https://user-images.githubusercontent.com/18084932/144856676-1527de09-58de-4b27-af47-2d70aa7fc46c.gif">
- 엑셀 입력
<img alt="ex" src="https://user-images.githubusercontent.com/18084932/144856899-06780a9b-4821-4be2-823f-a2cecdfcd75d.gif">
- 공지사항 및 운영시간 설정
<img alt="notice" src="https://user-images.githubusercontent.com/18084932/144857747-a47317b8-95d7-4fdf-b4fe-9ae3465c91fe.gif">

## 개발 목적

---
- Front와 Back-end를 분리를 통해 유지보수의 이점을 경험
- 개인 사업자(약국)가 보유하고 있는 약품의 재고와 정보를 WEB으로 표현해 Back-end와 Front-end의 전반적인 프로세스를 경험하기
- 보유하고 있는 일반 의약품의 정보를 쉽게 등록할 수 있는 솔루션을 구현


## 기획

---
*현 프로젝트는 일반 이용자(회원)이 이용하는 페이지가 아닌 관리자(개인 사업자)가 이용하는 admin 페이지를 구현*
- 자신의 매장의 재고 보유 목록을 웹 브라우저를 통해 손쉽게 업로드하고 개인 일정 등을 적어 놓을 수 있도록 구현

## 프로젝트 주요 기능

---
- 공지사항 및 운영시간 등록
- 바코드 인식을 통한 재고 등록
- 엑셀 파일을 통한 재고 등록
- restAPI 구현을 통한 데이터 등록 및 조회 구현
## 사용 기술

---
- 바코드 처리 관련 (해당 프로젝트에 포함 X - 따로 구현)
  - Python
  - Flask
  - ZBar

---
- SpringBoot 2.5
- Maven
- Mybatis
- MySQL
- Lombok
- Java 8
- Jsoup
---
- Bulma CSS Framework
- FullCalendar - JS Calendar 라이브러리
- Tabulator - JS Table 라이브러리
- SheetJS - JS Excel 라이브러리

## UseCase

---

~~~ 
일반 사용자
- 회원 가입
    - 회원 가입하기
    - 리뷰 남기기
    - 약국에 재고 요청하기
- 검색
    - 현재 위치 기반 근처 약국 검색
    - 약을 토대로 약국 검색
    - 지역 설정을 통해 약국 검색
- 약국 조회 ( 상세 페이지 )
    - 운영시간 확인
    - 재고 상태 확인
    - 공지사항 확인
    - 리뷰 작성
    - 희망 약품 신청
        - 다른 일반 회원들도 좋아요를 누를 수 있다.
- 마이 페이지
    - 복용 시간 등록
    - 복용 약 등록
~~~
### 관리자 ( 약국 사업자 - 개인 사업자 )

관리자는 매장의 정보를 관리한다

- 약국(매장) 관리
    - 운영시간 설정
        - 월 화 수 목 금 토 일
            - 특정 시간대를 지정해서 운영 시간을 설정 할 수 있다.
            - 휴무일 지정
    - 공지사항 설정
    - 일반 의약품 관리
        - 재고 등록
            - 엑셀
            - 바코드
        - 재고 삭제
---
## ERD

<img alt="ERD" src="https://user-images.githubusercontent.com/18084932/144841762-c07f5b88-0060-4bde-8c79-779dab9f23ab.png"> 

---
## Json 응답 데이터 및 DB 조회 결과
- 운영시간 및 공지사항 설정
<img alt="json" src="https://user-images.githubusercontent.com/18084932/144849880-865db3f4-3c15-4c08-8c11-3da5d4a863ba.png">
- 엑셀 데이터 추가 및 설정
<img alt="ex" src="https://user-images.githubusercontent.com/18084932/144850115-9f7e74fb-66ea-4e43-84b7-02e2c21a5e21.png">
- DB
  - 재고목록
     <img width="641" alt="테이블 캡처 1" src="https://user-images.githubusercontent.com/18084932/144850663-6927b902-b2bb-42d3-a2db-934c2111a071.PNG">
  - 공지사항 및 운영시간
    <img width="666" alt="테이블 캡처 2" src="https://user-images.githubusercontent.com/18084932/144850896-549cffb0-182f-462e-8303-24b77496afbe.PNG">
