# Movie Site (팀 프로젝트)

> 영화 탐색(랭킹/장르/상세) + 커뮤니티(게시판/댓글/이미지) + 예매 흐름을 제공하는 웹 서비스  
> **Spring Boot + Thymeleaf + Spring Security + JPA/MyBatis + MySQL**

---

## 1) 프로젝트 소개
사용자는 영화 랭킹/장르 기반으로 영화를 탐색하고, 상세 페이지에서 정보를 확인한 뒤  
상영 정보를 선택하여 예매할 수 있습니다.  
또한 커뮤니티(게시판/댓글/이미지 업로드) 기능으로 사용자 간 소통이 가능합니다.

---

## 2) 주요 기능

### 영화
- 랭킹/박스오피스/장르별 영화 목록
- 영화 상세 조회

### 회원/인증
- 회원가입 / 로그인 / 로그아웃
- 권한(일반/관리자) 기반 접근 제어

### 예매
- 상영 정보 선택 → 예매 진행 → 예매 완료 페이지
- 내 예매 내역 조회 / 취소

### 커뮤니티(게시판)
- 게시글 CRUD + 페이징
- 댓글 작성/수정/삭제
- 이미지 업로드 (게시글 첨부)

---

## 3) 기술 스택
- **Backend**: Java 17, Spring Boot, Spring MVC, Spring Security
- **Template**: Thymeleaf
- **DB**: MySQL
- **Data**: Spring Data JPA, MyBatis
- **Build**: Gradle

---

## 4) 내 역할 (팀 프로젝트)
> 아래는 예시입니다. 본인이 실제로 맡은 내용으로 수정하세요.

- 예매 도메인 설계 및 API 구현
- Spring Security 인증/인가 흐름 적용
- 게시판/댓글 기능 구현 및 페이징 처리
- 이미지 업로드 처리 및 예외/검증(Validation) 적용

---

## 5) 실행 방법(로컬)

### 1. MySQL DB 생성
```sql
CREATE DATABASE moviesite DEFAULT CHARACTER SET utf8mb4;

2. 설정 파일 작성
src/main/resources/application.properties에서 DB 계정 정보 수정

3. 실행
./gradlew bootRun

4. 접속
http://localhost:9090
