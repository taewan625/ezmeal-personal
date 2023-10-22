# ezmeal project
- 실제 구현한 페이지에 관련된 파일만 최대한 추출
- mapper, Controller, Service, Dao, Domain 패키지에 Java, SQL 코드 존재
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
1. 배송지  
![address](https://github.com/taewan625/ezmeal-personal/blob/master/%E1%84%87%E1%85%A2%E1%84%89%E1%85%A9%E1%86%BC%E1%84%8C%E1%85%B5.png)

2. 장바구니  
![cart](https://github.com/taewan625/ezmeal-personal/blob/master/%E1%84%8C%E1%85%A1%E1%86%BC%E1%84%87%E1%85%A1%E1%84%80%E1%85%AE%E1%84%82%E1%85%B5.png)

3. 배송지 관리  
![address](https://github.com/taewan625/ezmeal-personal/blob/master/%E1%84%87%E1%85%A2%E1%84%89%E1%85%A9%E1%86%BC%E1%84%8C%E1%85%B5.png)

4. 주문서  
![order](https://github.com/taewan625/ezmeal-personal/blob/master/%E1%84%8C%E1%85%AE%E1%84%86%E1%85%AE%E1%86%AB.png)

5. 주문 내역  
![orderList](https://github.com/taewan625/ezmeal-personal/blob/master/%E1%84%8C%E1%85%AE%E1%84%86%E1%85%AE%E1%86%AB%E1%84%82%E1%85%A2%E1%84%8B%E1%85%A7%E1%86%A8.png)

6. 주문 상세  
![orderDetail](https://github.com/taewan625/ezmeal-personal/blob/master/%E1%84%8C%E1%85%AE%E1%84%86%E1%85%AE%E1%86%AB%E1%84%89%E1%85%A1%E1%86%BC%E1%84%89%E1%85%A6.png)

7. 발주  
![barjoo](https://github.com/taewan625/ezmeal-personal/blob/master/%E1%84%87%E1%85%A1%E1%86%AF%E1%84%8C%E1%85%AE.png)

8. 배송준비  
![deliveryPrepare](https://github.com/taewan625/ezmeal-personal/blob/master/%E1%84%87%E1%85%A2%E1%84%89%E1%85%A9%E1%86%BC%E1%84%8C%E1%85%AE%E1%86%AB%E1%84%87%E1%85%B5.png)

9. 배송 중  
![deliverying](https://github.com/taewan625/ezmeal-personal/blob/master/%E1%84%87%E1%85%A2%E1%84%89%E1%85%A9%E1%86%BC%E1%84%8C%E1%85%AE%E1%86%BC.png)

10. 배송 완료  
![deliveryComplete](https://github.com/taewan625/ezmeal-personal/blob/master/%E1%84%87%E1%85%A2%E1%84%89%E1%85%A9%E1%86%BC%E1%84%8B%E1%85%AA%E1%86%AB%E1%84%85%E1%85%AD.png)

11. 로그인 모달  
<img src="https://user-images.githubusercontent.com/104051002/274786873-f6de4ef3-2aae-42de-9bfe-44e1350f8265.png" alt="image" style="width: 1000px;">

## reference
- WeEat, Kurly, Gmarket, Cafe24
- [Co](https://code-is-me.tistory.com/)https://code-is-me.tistory.com/
- 자바의 정석
- 노마드 코더
- 모던 딥다이브 자바스크립트
- 스프링의 정석
- 우아한형제들 최연소 기술이사 김영한의 스프링 완전 정복
