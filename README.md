# 안녕하세요김찬결입니다잘부탁드립니다

백엔드 프로젝트를 진행해왔고, 지금은 클라우드 엔지니어를 준비하고 있습니다.

Java와 Spring Boot로 서비스를 개발하면서  
애플리케이션 내부뿐 아니라 서버, 네트워크, 데이터베이스가  
실제 환경에서 어떻게 연결되어 동작하는지에 관심이 생겼습니다.

현재 Linux, Networking, AWS를 공부하고 있습니다.

📫 changul20141461@gmail.com

---

## Projects

### 🗺️ 여기도

> UMC 10기 팀 프로젝트 · Backend Developer  
> 2026.06.22 ~ 2026.08.14  
> 11인 팀 (Backend 5 / Frontend 4 / PM 1 / Designer 1)

지역의 문화·여행 정보를 탐색하고,  
방문 경험을 기록·공유하며 지역 소상공인과 여행자를 연결하는 서비스입니다.

백엔드에서 **소상공인 홍보, 사업자 인증, 장소 좋아요** 도메인을 담당했습니다.

#### 제가 한 일

- 국세청 API 기반 사업자 인증 및 인증된 사업장 기반 홍보글 권한 검증
- QueryDSL 기반 추천순·저장순 커서 페이지네이션 및 계층형 지역 조회
- 장소 좋아요 등록·취소 및 좋아요 출처 검증
- Fetch Join과 일괄 조회를 통한 연관 데이터 조회 개선

#### 개발하면서 해결한 문제

- `SELECT → INSERT` 방식의 좋아요 경쟁 조건을 `UNIQUE + INSERT IGNORE` 구조로 변경하고 10건의 동시 요청으로 중복 생성 방지 검증
- 국세청 인증 실패를 미등록·정보 불일치·외부 API 장애로 구분해 각각 다른 서비스 예외로 처리
- Soft Delete와 `place_id` UNIQUE 제약을 함께 고려해 삭제된 홍보글의 재등록 정책 구현
- 홍보글과 장소 데이터가 서로 어긋나는 것을 막기 위해 등록 이후 Place 변경 제한

**Stack**  
`Java` `Spring Boot` `Spring Security` `JPA` `QueryDSL` `MySQL` `Flyway`

**Links**  
[Backend Repository](https://github.com/yeogido/backend) ·
[PR #297](https://github.com/yeogido/backend/pull/297) ·
[PR #146](https://github.com/yeogido/backend/pull/146) ·
[PR #91](https://github.com/yeogido/backend/pull/91)

---

### 🏠 자취방 정보공유 플랫폼

> 데이터베이스 수업 팀 프로젝트 · DB 설계 담당

자취생들이 거주 경험과 방 정보를 공유할 수 있도록 설계한 커뮤니티 플랫폼입니다.

- 회원, 자취방, 리뷰, 좋아요, 거주 인증, 문의·답변 등의 ERD와 테이블 구조 설계
- 중복 좋아요 방지를 위한 관계 테이블 설계
- 거주 인증 여부와 사용자 유형에 따른 리뷰·답변 권한 구조 설계
- 팀 요구사항과 교수님 피드백을 반영하며 ERD 개선

**Stack**  
`MySQL`

---

## What I use

**Backend**  
Java · Spring Boot · Spring Security · JPA · QueryDSL

**Database**  
MySQL · Flyway

**Tools**  
Git · GitHub · Swagger

**Currently learning**  
Linux · Networking · AWS · Cloud Infrastructure

---

## Links

[GitHub](https://github.com/chans20)
