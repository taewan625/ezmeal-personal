# ezmeal project
- 실제 구현한 페이지에 관련된 파일만 최대한 추출
- 모든 서비스 로직은 https://github.com/taewan625/ezmeal-refactoring 에 존재

## 목차
  - [개요](#개요)
  - [기획](#기획)
  - [실행환경](#실행환경)
  - [구현기능](#구현기능)
  - [참조](#reference)

## 개요
- 프로젝트 이름   : ezmeal 쇼핑몰 프로젝트
- 프로젝트 기간   : 2023.05.30~2023.08.06 
- 개발 언어      : Java11, Spring Legacy, MyBatis, MySQL, JSP, CSS3, JavaScript(ES6), Ajax, JQuery
- 사용 tool     : IntelliJ, DataGrip, ERD Cloud, Git, GitHub
- 사용 외부 API  : 아임포트 결제 API

## 기획
- 기획의도 : 음식물 쇼핑물 사이트 개발 - 사용자 및 관리자 화면 개발

## 실행환경
- Tool : IntelliJ
- Language : Java11, Spring Legacy, MyBatis, MySQL, JSP, CSS3, JavaScript(ES6), Ajax, JQuery

## 구현기능
- 담당 ERD : 장바구니, 주문, 결제, 배송 관련 ERD 구축
- 담당 화면 : 장바구니, 주문, 결제, 배송, 배송지 화면 개발, 로그인 모달창 개발

### ERD (파란색)
<img src="https://user-images.githubusercontent.com/104051002/274786370-aeafafbb-435e-4975-8457-f5cfa821dd1a.png" style="width: 1000px;">

### 페이지별 구현
1. 장바구니
<img src="https://private-user-images.githubusercontent.com/104051002/274780957-bd58d191-e270-42b7-853e-529dd37c1f3e.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTEiLCJleHAiOjE2OTcxNjYyOTYsIm5iZiI6MTY5NzE2NTk5NiwicGF0aCI6Ii8xMDQwNTEwMDIvMjc0NzgwOTU3LWJkNThkMTkxLWUyNzAtNDJiNy04NTNlLTUyOWRkMzdjMWYzZS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBSVdOSllBWDRDU1ZFSDUzQSUyRjIwMjMxMDEzJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDIzMTAxM1QwMjU5NTZaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1lNjBlZmEwYTZiNjExN2QyZTZmMDZmYTU5NWVhODAzYzY1ODUxOGVkZWM1ZjQ1NjQ4MDE4OTI1NDMyMzJkYTNmJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.9GGhLTg5hkF6ct6ATQx0Rn48KB2bsVxk3f5fFYvGXHQ" alt="image" style="width: 1000px;">

2. 배송지 관리
<img width="1000" alt="image" src="https://user-images.githubusercontent.com/104051002/274786658-e1740787-5b6d-409a-afa3-392e79fd6ff8.png" style="max-width: 100%;">

3. 주문서
<img src="https://private-user-images.githubusercontent.com/104051002/274781256-7ff925a3-70d0-4409-9e0e-336eb97badfc.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTEiLCJleHAiOjE2OTcxNjY4ODksIm5iZiI6MTY5NzE2NjU4OSwicGF0aCI6Ii8xMDQwNTEwMDIvMjc0NzgxMjU2LTdmZjkyNWEzLTcwZDAtNDQwOS05ZTBlLTMzNmViOTdiYWRmYy5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBSVdOSllBWDRDU1ZFSDUzQSUyRjIwMjMxMDEzJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDIzMTAxM1QwMzA5NDlaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT00ODg1MzY5ZjIzZGMyZmMwMTMzYmFjNmVlOTI4NWU4YzZhZjYwMTBmNjRlMGRjMzY2ZTM1MTI0NWZiYThiMWVjJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.eYXcYpcRs04TMUwe54OjenffLNAe2bkL9qwrlPqvo5I" alt="image" style="width: 1000px;">

5. 주문 완료
<img src="https://private-user-images.githubusercontent.com/104051002/274781609-312986fb-fefd-4eb0-b863-75cf152e4eab.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTEiLCJleHAiOjE2OTcxNjY5NDEsIm5iZiI6MTY5NzE2NjY0MSwicGF0aCI6Ii8xMDQwNTEwMDIvMjc0NzgxNjA5LTMxMjk4NmZiLWZlZmQtNGViMC1iODYzLTc1Y2YxNTJlNGVhYi5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBSVdOSllBWDRDU1ZFSDUzQSUyRjIwMjMxMDEzJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDIzMTAxM1QwMzEwNDFaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1iNzI1NWFjYzUxMjAzOGU0ZjQ0Njc2YThlODczOTExN2ZiZjJiYzZhYTE1ZWMyMWI0YTY4OWZmODI2Y2NmNzRlJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.--jtCcHq1hs15f6FFD9AZeyiafv5MwMHmQEaTRU7soA" alt="image" style="width: 1000px;">

7. 주문 내역
<img src="https://private-user-images.githubusercontent.com/104051002/274781038-f9f7e19e-fa12-4020-b142-91f3be15b020.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTEiLCJleHAiOjE2OTcxNjY5NzUsIm5iZiI6MTY5NzE2NjY3NSwicGF0aCI6Ii8xMDQwNTEwMDIvMjc0NzgxMDM4LWY5ZjdlMTllLWZhMTItNDAyMC1iMTQyLTkxZjNiZTE1YjAyMC5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBSVdOSllBWDRDU1ZFSDUzQSUyRjIwMjMxMDEzJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDIzMTAxM1QwMzExMTVaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1mZDkwM2Q4NmJhMWI2Yjg4NzkwOWI3ZjFiNGU4MjRmMTQwNzVkZTVkYTljMzgyNTI2ZGU5OGQ2YTMyYzE3YjViJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.m3vs4ZGuqU1wnWpeiXThYYyfdr9j-KM9hKdiXaDUx34" alt="image" style="width: 1000px;">

9. 주문 상세
<img src="https://private-user-images.githubusercontent.com/104051002/274781171-59130a84-f462-4545-a07a-d34ebba32d3c.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTEiLCJleHAiOjE2OTcxNjY5OTQsIm5iZiI6MTY5NzE2NjY5NCwicGF0aCI6Ii8xMDQwNTEwMDIvMjc0NzgxMTcxLTU5MTMwYTg0LWY0NjItNDU0NS1hMDdhLWQzNGViYmEzMmQzYy5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBSVdOSllBWDRDU1ZFSDUzQSUyRjIwMjMxMDEzJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDIzMTAxM1QwMzExMzRaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT0wZWExZTJlZTgwMDc3ZDI5YmJlYWU2NzgyMzk4MTAwNTI4YmUyMzc1NzhmZWMyZGE0MzI2MmFkZWZjMzRmYzMxJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.TIgFWcjkGlgGIj620KuIIy8JPv_IIPUhcP2if3vm8JM" alt="image" style="width: 1000px;">

11. 배송준비중 관리
<img src="https://private-user-images.githubusercontent.com/104051002/274781404-1fdb36c9-9e17-471a-a12d-18e62fc71e2c.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTEiLCJleHAiOjE2OTcxNjcwMDksIm5iZiI6MTY5NzE2NjcwOSwicGF0aCI6Ii8xMDQwNTEwMDIvMjc0NzgxNDA0LTFmZGIzNmM5LTllMTctNDcxYS1hMTJkLTE4ZTYyZmM3MWUyYy5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBSVdOSllBWDRDU1ZFSDUzQSUyRjIwMjMxMDEzJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDIzMTAxM1QwMzExNDlaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT02ODc4Y2RjOWYyMjU3YjVkY2I4NjJiNGZiOTE5OWViMzJlZmE3ZGU2MTIwYWIzNzkyZmExODZhMDZkZTE5ZmM1JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.fahJrR25-57iPIxvm2BOTkbtbnbQhLrjCk3DuefEM3E" alt="image" style="width: 1000px;">

13. 배송중 관리
<img src="https://private-user-images.githubusercontent.com/104051002/274781535-a5fdc52c-536d-4af4-845d-5b6c8e9a4f4d.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTEiLCJleHAiOjE2OTcxNjcwMDksIm5iZiI6MTY5NzE2NjcwOSwicGF0aCI6Ii8xMDQwNTEwMDIvMjc0NzgxNTM1LWE1ZmRjNTJjLTUzNmQtNGFmNC04NDVkLTViNmM4ZTlhNGY0ZC5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBSVdOSllBWDRDU1ZFSDUzQSUyRjIwMjMxMDEzJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDIzMTAxM1QwMzExNDlaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT02MjhmMjMxNTM3YjZlYjY5MDcyZmIxNDliYzY2NWIwMjc1ZjIxZTY5ZmQ2NWEzMGMxOGI1YTI3YWNjYmJmYjMyJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.hIjC8pCePdMfRCizAaAjR4Z1Ft20AWzAOIo3jYvYS-A" alt="image" style="width: 1000px;">

15. 배송완료 조회
<img src="https://private-user-images.githubusercontent.com/104051002/274781551-0e8c522b-41dd-4f94-ad6e-1a6fd2dd0d5d.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTEiLCJleHAiOjE2OTcxNjcwMDksIm5iZiI6MTY5NzE2NjcwOSwicGF0aCI6Ii8xMDQwNTEwMDIvMjc0NzgxNTUxLTBlOGM1MjJiLTQxZGQtNGY5NC1hZDZlLTFhNmZkMmRkMGQ1ZC5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBSVdOSllBWDRDU1ZFSDUzQSUyRjIwMjMxMDEzJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDIzMTAxM1QwMzExNDlaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1hOTExMDIwM2U2NWE0ZGRiM2QwNzY5NjEyMTkzNWUzNjg3MjA2Y2NiY2JmZGM4NjNjY2NhOWYyNzliYzY0MzUxJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.7I3bP9CK3eSzSwVCBvb2c2rgntcbXBYwuabYexrsxRc" alt="image" style="width: 1000px;">

16. 로그인 모달 
<img src="https://user-images.githubusercontent.com/104051002/274786873-f6de4ef3-2aae-42de-9bfe-44e1350f8265.png" alt="image" style="width: 1000px;">

## reference
- WeEat, Kurly, Gmarket, Cafe24
- [Co](https://code-is-me.tistory.com/)https://code-is-me.tistory.com/
- 자바의 정석
- 노마드 코더
- 모던 딥다이브 자바스크립트
- 스프링의 정석
- 우아한형제들 최연소 기술이사 김영한의 스프링 완전 정복
