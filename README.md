# Spring MVC 쇼핑몰

## 개발 동기
- 평소 패션에 관심이 많은 저는, 무신사를 보며 이와 같은 Web을 구축해보고 싶었고, 그에 따라서 쇼핑몰이라는 주제를 선정하게 되었습니다.
- 실제로 많은 기업들에서 사용자에게 서비스를 제공하는 sales web site를 구축해보고, 도메인부터 아키텍처까지 이해하며 습득하는 것이 프로젝트의 큰 목표입니다.
- 제가 평소에 관심이 있던 기술 스택들을 구현하며 궁금증을 해소하고, 기술을 습득하고자 시작하게 되었습니다

## ⚒️Skill Stack
- Front-end
    - HTML ,CSS, Thymeleaf
- Back-end
    - JAVA, Spring, Spring Security, Spring Data JPA, Querydsl
- DB
    - MySQL8
## 프로젝트 구현 기능
- Member
    - 로그인
    - 회원가입
- Item
    - 상품 등록
    - 상품 관리
    - 상품 수정
    - 상품 상세
- Cart
    - 담기
    - 조회
    - 수정
    - 삭제
    - 주문
- Order
    - 단일 상품 주문
    - 주문 내역 조회
    - 주문 취소
## ERD
![Untitled (1)](https://github.com/dujong/shopping_mall/assets/55770741/494d1680-0d4b-472d-b999-8bece639f936)

## API 명세서
| Group | Function | Method | End Point |
| --- | --- | --- | --- |
| 홈 | 메뉴 View | GET | / |
| 회원 | 로그인 | GET | /login |
|  | 회원가입 | POST | /new |
| 상품 | 상품 등록 | POST | /admin/item/new |
|  | 상품 관리 | GET | "/admin/items", "/admin/items/{page}" |
|  | 상품 수정 | PUT | /admin/item/{itemId} |
|  | 상품 삭제 | DELETE | /item/{itemId} |
| 장바구니 | 장바구니 담기 | POST | /cart |
|  | 장바구니 조회 | GET | /cart |
|  | 장바구니 수정 | PUT | /cartItem/{cartItemId} |
|  | 장바구니 삭제 | DELETE | /cartItem/{cartItemId} |
|  | 장바구니 상품 주문 | POST | /cart/orders |
| 주문 | 단일 상품 주문 | POST | /order |
|  | 주문 내역 조회 | GET | "/orders", "/orders/{page}" |
|  | 주문 취소 | POST | /order/{orderId}/cancel |
