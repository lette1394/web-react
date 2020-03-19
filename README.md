# 옥나리

[TOC]

## 뭐하는 서비스인가요?

- 온라인 경매 사이트
- 실시간 채팅을 통해 참여자와 대화하며 경매 가능
- 자동 경매와 한도금액 설정을 통해 편하게 경매에 참여 가능

## 유스케이스

[경매 참고](https://namu.wiki/w/eBay#s-5.3)

<details>
<summary>자세히</summary>

### 메인 페이지

- 로그인
  - 로그인을 누르면 로그인 페이지로 이동한다.
- 마이페이지
  - 버튼을 누르면 마이페이지로 이동한다.
- 상품 나열
  - 메인페이지는 카테고리별로 정렬된 아이템을 보여준다.
  - 보여주는 정보는 상품명, 사진, 현재 입찰가, 남은 경매 시간을 보여준다.
  - 상품을 누르면 경매페이지로 넘어간다.
- 검색
  - 사용자는 경매할 물품을 검색 input 을 통해 검색할 수 있다.
  - 기본적으로 추천검색어를 보여주고 사용자의 입력이 들어 올 시 유사단어, 추천검색어를 보여준다.
- 카테고리
  - 카테고리는 (HOT 아이템, 시간임박, 전체보기(기본)), (상품종류 ex: 전자제품, 생필품, 가구 등을 세분화하여 카테고리분류)

### 로그인 페이지

- Oauth 로그인 방법을 선택한다. (카카오, 네이버, 구글, 페이스북)
- 인증이 성공하면 회원가입 페이지로 이동한다.

### 마이 페이지

- 개인정보 수정 가능
- 관심상품 확인 가능
- 현재 입찰 상품 확인 가능

### 회원가입 페이지

- 입력해야 할 정보는 최소한으로(결제 정보를 넣을지 말지 고민)
- 아이디 찾기 비밀번호 찾기는 없음

### 경매 페이지

- 경매
  - 보여지는 UI는 1.상품명, 2.사진, 3.시작가, 4.현재 입찰가, 5.호가, 6.남은 경매 시간, 7.등록 날짜, 8.종료 날짜, 9.입찰자, 10.카테고리, 11.입찰 참여자 수
  - 경매 참여 UI는 금액을 적는 input과 입찰 버튼, 자동입찰버튼으로 구성
  - 금액을 입력 후 입찰 버튼을 누르면 해당 금액으로 바로 입찰이 된다.
  - 금액을 입력 후 자동경매버튼을 누르면 다른 사람이 높은 금액으로 입찰할 경우 입력한 금액까지 한 호가 더 높은 금액으로 자동 입찰한다.
  - 두 명 이상의 사람이 자동입찰기능을 사용한경우 가장 높은 가장 높은 금액을 임력 한 사람이 그보다 낮게 설정한 사람보다 한 호가 더 높은 금액으로 입찰하게 된다.
  - 자동입찰을 한 경우 자동입찰버튼은 자동입찰 취소버튼으로 변하며 색도변한다.
- 채팅
  - 닉네임을 기반으로 다른 사용자와 실시간 채팅 가능
  - text input과 전송버튼으로 입력(엔터로 대체 가능)
  - 도배 방지를 위해 최대100byte 길이의 메세지만 허용, 5초에 3번 이상 채팅 불가
  - 현재 입찰자의 아이디는 색깔로 강조, 과거 입찰자의 아이디는 다른 색깔로 강조

### 알림

- 자신이 입찰한 물품에 다른 사람이 입찰했음을 알리는 알림(피드), 바로 알려주도록 함
- 관심상품으로 등록한 물품의 가격에 대한 알림, 과열 상품의 경우 알림이 많아질 수 있으므로 방지를 위한 방법 필요

</details>

## 프로젝트 구조

https://cloudcraft.co/

## 테스트 및 문서 설계

(단위테스트, 통합테스트는 어떻게 할건지, 문서화는 어떻게 할건지)

## 자랑

- 모바일 환경 지원

## 기술 스택

<details>
<summary>접기/펼치기 버튼</summary>

## Spring Boot vs Node.js

## React vs Other Framework

## Typescript

## RDBMS vs NOSQL

## BootStrap vs Material UI vs Styled-Components

## Redis

## Kafka vs RabbitMQ

## GraphQL

## Jenkins vs Travis vs Github Action vs Ant Design

## WebSocket

## Docker

## Mocha vs Jest

</details>
