# **다양한 기술과 경험을 토대로 빠르게 프로젝트에 기여할 수 있는 역량을 갖춘 개발자입니다.**

## 오제하

Java, Spring 환경의 백엔드 개발 포지션을 주로 담당하였으며, 프론트엔드 및 인프라 개발에도 관심이 있습니다.  
레거시 프로젝트 개선, 신규 프로젝트 설계 및 고도화 개발에도 참여하였습니다.  
기술 중심 사고와 더불어 현 프로젝트 상황을 파악하여 최적화된 개발 방법과 기술을 적용하여 문제를 해결하는 것을 중요하게 생각합니다.  
  

## Contact

- jeaha1217@gmail.com
- 010 5592 6282

## Channel

- https://jeaha.dev
- https://github.com/JeahaOh

## 강점

- 레거시 프로젝트의 기능개선, 유지보수 경력으로 java / spring 프로젝트에 바로 기여 가능합니다.
- 조직의 비즈니스 성장을 위한 원활한 의사소통이 가능합니다.
- 단단한 성장을 위해 지속적이고 주도적인 학습을 합니다.

## Skills

### Main

- Java(1.7 - 11)
- Spring Framework, Spring Boot
- JavaScript

### Sub / Infra

- Oracle DB, PostgreSQL, MySQL
- Tomcat, Nginx, Apache HTTPD
- Linux, AWS(EC-2, S3, CloudFront, CloudWatch, CodeDeploy)

### Tools

- Jira, Confluence
- Git, GitHub
- Maven, Jenkins, Slack

<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

---

## 경력

- 아이디룩
  - 이커머스 개발팀 주임
  - 2021.08.23 ~ 재직 중 (2 년 2 개월)
  - 자사 쇼핑몰 웹 서비스 운영 및 회원/이벤트/전시/배송 파트 고도화
  - 최대 5,700명 동시 접속, 일 최대 4.2만 명 접속, 월 최대 44만 명 접속
  - 현 상황에 적절한 기술을 이용하여 성능과 유지보수성, UX 향상, 기술 부채 감소. 매출 증대에 기여.
  - 패션 제조 / 유통, 연 매출 2080 억, 영업 이익 150억, 170 명 (2022 년)
- 한신정보기술
  - 개발 3팀 사원
  - 2020.11.02 ~ 2021.08.19 (9 개월)
  - 공공기관 홈페이지 유지보수 및 기능 고도화
  - IT 외주, 연 매출 60억, 100 명 (2021 년)
- 지엠티
  - 서비스개발팀 사원
  - 2019.05.20 ~ 2020.10.31 (1 년 5 개월)
  - 공공기관 업무 포털 공간정보 기능 개발 및 유지보수
  - 적극적인 커뮤니케이션 능력을 활용하여 다양한 니즈 파악 및 솔루션 고도화에 기여
  - Web Application, DB, Infra 전반에 걸친 운영 및 성능 개선
  - IT 솔루션 제공, 연 매출 300억, 140 명 (2020 년)

<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

---

## 프로젝트 수행 내역

### 아이디룩

#### 이벤트 상품 목록 조회 성능 고도화

- 2023.07.24 ~ 2023.08.17
- Redis를 사용하여 이벤트 페이지 하위 상품 목록의 조회성능 개선.
- DB CPU 사용율 감소와 그에 따른 소화 가능 트래픽 증가.

#### 스케쥴러 시스템 고도화

- 2023.05.08 ~ 2023.05.26
- Spring + Quartz로 작동하던 스케쥴링 작업을 Spring Batch + Jenkins로 이관
- 여러개의 Step 구동 및 실행 상태에 따른 분기처리.

#### 조회 쿼리 성능 개선

- 2023.03.27 ~ 2023.04.15
- 상품 목록 조회 쿼리의 실행 비용을 {4,095 CPU COST, 24,418 BUFFERS}에서 {1,047 CPU COST, 12,913 BUFFERS}으로 개선.
- Oracle Query Hint와 GATHER_PLAN_STATISTICS을 이용하여 실제 쿼리 성능을 분석.

#### 물류/배송 시스템 개편

- 2022.10.03 ~ 2023.01.15
- 3자물류 연계 기능 개발로 배송팀 공수 감소
- Spring 프로젝트에 Quartz로 스케쥴링하여 3자 물류 연계 기능 자동화. (재고관리, 결품관리, 출고/반품 배송 신청/실적 관리 기능 등)
- API 통신시 요청 경로, 파라미터, 응답 값, 요청/응답 시간을 별도로 저장하기 위해 Spring AOP 기능을 이용함.

#### 대용량 데이터 처리 기능 고도화

- 2022.08.15 ~ 2022.08.31
- 하루 평균 3,000 건의 배송을 추적하는 기능의 고도화로 수행시간의 60% 감소.
- Spring Async Annotation으로 비동기 멀티스레드 구현.
- MyBatis Execute type BATCH 옵션과 Transactional Annotation의 REQUIRED_NEW 속성으로 트랜젝션 관리.

<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

#### 이벤트 / 프로모션 기능 고도화 (통합프로모션)

- 2022.07.01 ~ 2022.08.12
- 마케팅 기능 콘텐츠(쿠폰 다운로드, 사다리타기, 응모, 랜덤 뽑기, 추첨 등)가 한 번에 한 개만 생성할 수 있던 것을 페이지 안에서 여러 콘텐츠를 포함할 수 있도록 구조 개선.
- Spring Framework 기반 JAVA RESTful API을 개발하여 이벤트/프로모션 기능 통합, 개발/마케팅/MD 팀의 공수 5일 감소.

#### AWS 전환

- 2022.01.12 ~ 2022.04.21
- Redis와 Spring Framework를 연동하여 Session Clustering 구성으로 사용자 UX 개선, 관련 CS 인입 감소
- 절차지향으로 개발되어 파편화된 파일 관리 로직을 S3 파일 관리 클래스로 분리하여 단일 책임수행과 유지보수성 향상 도모.
- IDC CDN 서비스를 AWS Cloud Front 서비스로 전환, 월평균 160만 원 비용 절감
- 수기 배포에서 Jenkins를 활용한 배포 자동화 전환. 배포 시간을 1시간에서 10분으로 개선.

#### 웹 성능 최적화

- 2021.10.01 ~ 2021.10.15
- 클라이언트 요청에서 화면 렌더링까지 10초 이상 (피크타임 기준) 걸리던 화면을 최적화하여 2초 내외로 개선
- CDN, Gzip 사용, JS/CSS 파일의 minify, 이미지 리싸이즈, 지연로딩 등 정적 콘텐츠 최적화
- 메인 페이지, 프로모션 페이지 요청시 조회하는 일부 데이터를 redis에 cache 저장하여 응답 속도 개선
- 프로모션 하위 상품 목록의 페이징 처리

<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

---

### 한신정보기술

#### 하남시청 유지보수 및 고도화

- 2020.11.29 ~ 2021.08.19
- Linux crontab scheduler를 이용하여 프로세스 다운시 자동 재실행, 관리자에게 알림을 발송하여 장애관리 도모
- JVM GC 튜닝으로 빈번하게 다운되는 WAS 문제 해결
  
---
  
### 지엠티

#### 해양환경공단 골재채취선박 및 해양환경 관제 시스템 개발

- 2019.10 ~ 2020.08
- Vanilla JavaScript와 OpenLayers를 이용하여 해양지도 SPA 개발
- Java 1.8과 Spring 4.1을 이용하여 RESTfull API 설계 및 구현

#### 해양 GIS 데이터 정제

- 2019.10 ~ 2019.10
- 대한민국 바다에서 선박들이 분당 2회씩 수신한 항해 데이터 10년치, 약 25,920,000,000 건을 해양대에서 연구할 수 있도록 파싱하여 DB에 저장하도록 데이터 모델링 및 프로그램 개발.
- Java와 MyBatis를 이용, 암호화된 데이터를 파싱하여 객체로 읽어 들이는 비즈니스 로직과 데이터를 비동기, bulk insert 하여 10,000 건씩 삽입하는 로직으로 분리하여 개발.
- 년, 월 별로 table을 파티셔닝하여 데이터를 저장하도록 설계.