# 안녕하세요, 백엔드 개발 경험을 쌓고 있는 김찬결입니다 👋

Java와 Spring Boot를 기반으로 서비스를 개발하며,
문제의 원인을 파악하고 데이터 정합성과 안정성을 개선하는 과정에 관심이 있습니다.

<br>

## 🙋 About Me

- 🌱 Java와 Spring Boot 기반의 백엔드 개발 경험을 쌓으며, 안정적인 서비스 구조와 데이터 처리에 관심을 두고 있습니다
- 💡 기능 구현에 그치지 않고 동시성, 데이터 정합성, 조회 성능, 예외 처리의 원인을 분석하고 개선하는 과정을 중요하게 생각합니다
- ☁️ 백엔드 개발 경험을 기반으로 네트워크, Linux, AWS를 학습하며 클라우드 영역으로 역량을 확장하고 있습니다
- 📫 Contact: changul20141461@gmail.com

<br>

## 🛠 Tech Stack

### Backend

![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=java&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white)
![Spring Data JPA](https://img.shields.io/badge/Spring_Data_JPA-59666C?style=flat-square)
![QueryDSL](https://img.shields.io/badge/QueryDSL-0769AD?style=flat-square)

### Database

![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Flyway](https://img.shields.io/badge/Flyway-CC0200?style=flat-square&logo=flyway&logoColor=white)

### Language

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=white)

### Tools

![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=flat-square&logo=swagger&logoColor=black)

<br>

## 💡 Skills

| 분야 | 경험 |
|------|------|
| **Backend** | Java/Spring Boot 기반 REST API와 도메인 비즈니스 로직 구현 |
| **Database** | JPA·QueryDSL을 활용한 동적 조회, 커서 페이지네이션, Fetch Join 및 일괄 조회 경험 |
| **Data Integrity** | MySQL UNIQUE·CHECK 제약, Soft Delete, 트랜잭션을 고려한 데이터 정합성 처리 |
| **API Integration** | 외부 API 연동 및 응답·장애 유형을 서비스 예외로 변환하는 로직 구현 |
| **Collaboration** | Git Flow 기반 Issue → Branch → PR → Code Review → Merge 협업 경험 |

<br>

## 📊 GitHub Stats

![GitHub stats](https://github-readme-stats.vercel.app/api?username=chans20&show_icons=true&theme=default)

<br>

## 📁 Projects

### 🗺️ 여기도
> UMC 10기 팀 프로젝트 | Backend Developer  
> 2026.06.22 ~ 2026.08.14 | 11인 팀 (BE 5 / FE 4 / PM 1 / Designer 1)

지역의 문화·여행 정보를 지도에서 발견하고, 방문 경험을 기록·공유하며  
지역 소상공인과 여행자를 연결하는 로컬 문화 아카이빙 플랫폼

**기술 스택**

![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=java&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![JPA](https://img.shields.io/badge/JPA-59666C?style=flat-square)
![QueryDSL](https://img.shields.io/badge/QueryDSL-0769AD?style=flat-square)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)

**역할 및 기여**
- 소상공인 홍보, 사업자 인증, 장소 좋아요 도메인의 REST API 및 비즈니스 로직 담당
- 국세청 API 기반 사업자 인증과 인증된 본인 사업장 기반 홍보글 등록 권한 검증 구현
- QueryDSL 기반 추천순·저장순 복합 커서 페이지네이션 및 계층형 지역 필터 구현
- 작성자 Fetch Join과 페이지 단위 연관 데이터 일괄 조회를 적용해 N+1 조회 방지

**문제 해결 과정**
- 좋아요 등록의 `SELECT → INSERT` 경쟁 조건을 DB의 `UNIQUE` 제약과 `INSERT IGNORE`로 개선하고, API도 상태 설정의 의미에 맞게 `POST → PUT`으로 변경. 동일 사용자·장소에 10건의 동시 요청을 보내 중복 생성 방지 검증
- 국세청 `/validate` 실패 시에만 `/status`를 추가 조회해 미등록·영업 상태 문제와 입력 정보 불일치를 구분하고, 국세청 통신 장애는 별도 `503` 오류로 처리
- `place_id` UNIQUE 제약과 Soft Delete 정책을 함께 고려해 동일 장소 재등록 시 기존 행을 재활성화하고, 홍보 콘텐츠와 장소 데이터의 불일치를 막기 위해 등록 이후 Place 변경을 제한

**GitHub**
- [Backend Repository](https://github.com/yeogido/backend)

<br>

### 🏠 자취방 정보공유 플랫폼
> DB 수업 팀 프로젝트 | DB 설계 담당

자취생들이 거주 경험을 공유하고 방 정보를 탐색할 수 있는 커뮤니티 플랫폼

**기술 스택**

![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)

**주요 기능**
- 게시글 등록, 리뷰 작성, 좋아요, 거주 인증, 문의/답변, 주변 편의시설 정보 제공

**역할 및 기여**
- 회원, 자취방, 리뷰, 좋아요, 거주 인증, 문의/답변 등 전체 ERD 및 테이블 구조 설계
- 팀원들과 기능 요구사항을 직접 질의응답하며 설계에 반영
- 교수님 피드백을 바탕으로 ERD 구조 개선

**문제 해결 과정**
- 좋아요 기능 설계 시 중복 방지와 취소 기능을 고려해 `Like_Residence(user_id, residence_id, liked_at)` 중간 테이블로 구조화
- 리뷰는 거주 인증된 사용자만 작성 가능하다는 규칙을 `Tenancy_Certification` 관계형 엔터티로 표현
- 답변 작성 권한을 `user_type` 컬럼으로 구분해 집주인/공인중개사만 답변 가능하도록 설계

<br>

## 🔗 Links

- 📁 GitHub: [github.com/chans20](https://github.com/chans20)
- ✍️ Blog: (작성 예정)
