# Spring Boot Bucket4j

## 1. 설명
Spring Boot Bucket4j 예제이다. 포트는 8080을 사용한다.

버킷의 크기는 3개이며 10초에 3개의 토큰을 충전한다.

API 호출시 토큰 1개를 소비한다.

## 2. 개발환경

* OpenJDK 17

* spring-boot 3.2.2

* bucket4j-core 8.7.1

* Gradle 8.5

## 3. API 실행
버킷을 모두 사용하면 토큰이 충전되기 전까지 조회 실패(TOO_MANY_REQUESTS)를 리턴한다.

* GET
  - http://localhost:8080/bucket
