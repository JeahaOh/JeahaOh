# Fact And Lesson in my career

## 이벤트 상품 목록 조회 성능 고도화

- FACT
  - Redis를 사용하여 이벤트 페이지 하위 상품 목록의 조회성능 개선.
  - DB CPU 사용율 감소와 그에 따른 소화 가능 트래픽 수 증가.
- LESSON
  - Legacy Spring, Java에서 Cache관련 Annotation을 사용할 수 없었고, Redis를 다루기 위해 유틸을 직접 만들었음.
  - Legacy System에서도 방법을 찾는다면 신기술을 사용할 수 있음을 경험함.
  - 레파토 법칙의 실제 사례를 겪어봄.
  - SQL로 모든 것을 해결하려 하면 안된다는 것을 재각인 함.
  - Web Application의 구조에서 DB 자원의 소중함을 경험하게 됨.

## 스케쥴러 시스템 고도화

- FACT
  - Spring + Quartz로 작동하던 스케쥴링 작업을 Spring Batch + Jenkins로 이관
- LESSON
  - 첫 Spring Boot, Spring Batch 실무 프로젝트
  - Jenkins로 스캐쥴링하여 Process를 실행하는 경험.

## 조회 쿼리 성능 개선

- FACT
  - 쿼리 실행 비용을 {4,095 CPU COST, 24,418 BUFFERS}에서 {1,047 CPU COST, 12,913 BUFFERS}으로 개선.
- LESSON
  - Oracle Query Hint와 GATHER_PLAN_STATISTICS을 이용하여 실제 쿼리 성능을 분석하는 방법을 경험.
  - RDBMS에서의 줄일 수 있는 자원은 여러가지가 있고, 쿼리의 목적에 따라서 방향이 다름을 배움.

## 물류/배송 시스템 개편

- FACT
  - 3자물류 연계 기능 개발로 배송팀 공수 감소
  - Spring 프로젝트에 Quartz로 스케쥴링하여 3자 물류 연계 기능 자동화. (재고관리, 결품관리, 출고/반품 배송 신청/실적 관리 기능 등)
  - API 통신시 요청 경로, 파라미터, 응답 값, 요청/응답 시간을 별도로 저장하기 위해 Spring AOP 기능을 이용함.
- LESSON
  - AOP 기능을 처음부터 사용하여 제대로 사용해 본 것은 처음.

## 대용량 데이터 처리 기능 고도화

- FACT
  - 하루 평균 4,000 건의 배송을 추적하는 기능의 고도화.
  - Spring Async Annotation과 MyBatis Execute type BATCH 기능으로 처리하여 소요시간 약 60% 감소.
- LESSON
  - Spring Async Annotation과 Async Thread Pool 관련 Spring 비동기 처리의 경험을 얻었음.
  - Transaction의 부모 자식 관계와 예외처리 경험.
  - 절차지향적으로 개발된 Legacy 코드를 객체지향 구조로 개선함.

## 이벤트 / 프로모션 기능 고도화 (통합프로모션)

- FACT
  - 마케팅 기능 콘텐츠(쿠폰 다운로드, 사다리타기, 응모, 랜덤 뽑기, 추첨 등)가 한 번에 한 개만 생성할 수 있던 것을 페이지 안에서 여러 콘텐츠를 포함할 수 있도록 구조 개선.
  - 이벤트/프로모션 기능 통합, 개발/마케팅/MD 팀의 공수 5일 감소.
- LESSON
  - 모듈화와 확장성을 고려한 설계의 중요성을 깨달음

## AWS 전환

- FACT
  - Redis와 Spring Framework를 연동하여 Session Clustering 구성으로 사용자 UX 개선, 관련 CS 인입 감소
  - 절차지향으로 개발되어 파편화된 파일 관리 로직을 S3 파일 관리 클래스로 분리하여 단일 책임수행과 유지보수성 향상 도모.
  - IDC CDN 서비스를 AWS Cloud Front 서비스로 전환, 월평균 160만 원 비용 절감
  - 수기 배포에서 Jenkins를 활용한 배포 자동화 전환. 배포 시간을 1시간에서 10분으로 개선.
- LESSON
  - 기술부채의 무서움을 배움.
  - 클린코드와 리팩토링의 중요성을 깨달음.
  - OOP의 원칙중 SRP의 중요성을 몸소 체험함.
  - Jenkins 설치부터 설정까지의 경험.
  - Redis, AWS EC-2, AWS S3, AWS Cloud Front에 대한 첫 실무 경험

## 웹 성능 최적화

- FACT
  - 클라이언트 요청에서 화면 렌더링까지 10초 이상 (피크타임 기준) 걸리던 화면을 최적화하여 2초 내외로 개선
  - CDN, Gzip 사용, JS/CSS 파일의 minify, 이미지 리싸이즈, 지연로딩 등 정적 콘텐츠 최적화
- LESSON
  - 네트워크와 웹 성능최적화 방법, 어플리케이션 동작의 효율성 향상을 통한 성능향상의 경험

## XX 시청 유지보수 및 고도화

- FACT
  - Linux crontab scheduler를 이용하여 프로세스 다운시 자동 재실행, 관리자에게 알림을 발송하여 장애관리 도모
  - JVM GC 튜닝으로 빈번하게 다운되는 WAS 문제 해결
- LESSON
  - JVM과 GC에 대한 이해를 얻음.
  - Linux OS와 친해짐.

## 해양환경 관제 시스템 개발

- FACT
  - Vanilla JavaScript와 OpenLayers를 이용하여 해양지도 SPA 개발
  - Java 1.8과 Spring 4.1을 이용하여 RESTfull API 설계 및 구현
- LESSON
  - RESTfull API의 설계 원칙에 대한 배움을 얻음.
  - Library, Framework의 중요성과 학습의 이유, 탄생 배경을 경험.

## 해양 GIS 데이터 정제

- FACT
  - 대한민국 바다에서 선박들이 분당 2회씩 수신한 항해 데이터 10년치, 약 25,920,000,000 건의 데이터를 DB에 저장하도록 데이터 모델링 및 프로그램 개발.
  - Java와 MyBatis를 이용, 암호화된 데이터를 파싱하여 객체로 읽어 들이는 비즈니스 로직과 데이터를 비동기, bulk insert 하여 10,000 건씩 삽입하는 로직으로 분리하여 개발.
- LESSON
  - 대용량 데이터를 저장하기 위한 파티셔닝 설계 방법을 배움.
  - MyBatis Batch 처리 방법와 Transaction 관리 방법의 경험.