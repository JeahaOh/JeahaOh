# 오제하

Java, Spring 환경의 BE 개발 경험을 가진 3년차입니다.  
Spring 개발을 가장 선호하며 FE 개발과 인프라 영역까지 개발/유지보수 가능합니다.  
신규 프로젝트 개발과 레거시 프로젝트 전환 그리고 개발, 설계, 기획을 포함한 경험이 있습니다.  
기술 중심 사고보다는 현재 상황을 파악하여 가장 적절한 개발 방법, 기술을 적용해 문제를 해결하는 것을 중요하게 생각합니다.  
  

## Contact

- jeaha1217@gmail.com
- 010 5592 6282
- https://jeaha.dev/
- https://github.com/JeahaOh

## 강점

- 레거시 프로젝트의 기능개선, 유지보수 경력으로 java / spring 프로젝트에 바로 기여 가능합니다.
- 사용자의 요구사항 파악을 위한 원활한 의사소통이 가능합니다.
- 프로젝트의 문서화와 사용자 메뉴얼 작성을 잘 합니다.
- 단단한 성장을 위해 지속적이고 주도적인 학습을 합니다.

## Skills

### Main

- Spring Framework
- Java(1.7 - 1.8)
- JavaScript

### Sub / Infra

- Oracle DB, MySQL, PostgreSQL
- Tomcat, Apache HTTPD, Nginx
- Linux, AWS(S3, CloudWatch, CodeDeploy)

### Tools

- Jira, Confluence
- Git, GitHub
- Maven, Jenkins, Slack

## 경력

- 아이디룩
  - 이커머스 개발팀 주임
  - 2021.08.23 ~ 재직중
  - 자사 웹 서비스 기능개선 및 유지보수
- 한신정보기술
  - 개발 3팀 사원
  - 2020.11.02 ~ 2021.08.19 (9 개월)
  - 공공기관 홈페이지 유지보수 및 기능개선
- 지엠티
  - 서비스개발팀 사원
  - 2019.05.20 ~ 2020.10.31 (1 년 5 개월)
  - 공간정보 기반 공공기관 업무 포털 기능개발 및 유지보수

## 프로젝트 수행 내역

### 아이디룩

- 자사 쇼핑몰(아이디룩몰, 아페쎄몰) 기능개선 및 유지보수
- 물류/배송 시스템 개편 (배송 시스템 모듈화, CJ Fulfillment)
- 대용량 데이터 처리 기능 개선 (SQL Session BATCH)
- 아페쎄몰 추가구성상품
- 이벤트/프로모션 기능 개선 (통합프로모션)
- OS File System 및 static resources의 S3 전환
- 리펙토링
- 스펙
  - BE : Java 1.7, Spring 3.1.1, myBatis, Oracle 11g
  - FE : jQuery 1.1
  - INFRA : AWS EC-2, AWS S3, AWS CodeDeploy, AWS CloudFront, Jenkins, NginX, Tomcat 8

#### 이벤트 기능 구조화

#### AWS 전환

- redis session
- OS FileSystem -> S3 API
- 정적 콘텐츠 배포의 CloudFront 전환

#### 수기업무의 기능화

- 월 정산
- 마켓팅 수신용 고객 데이터 추출

#### SVN -> GIT 전환

#### 오프라인 매장에서 QR 코드를 통한 통합회원 가입

#### 물류시스템 개선

- 택배사 전환
- CJ 풀필먼트

#### 추가구성상품

### 한신정보기술

- 2020.11.02 ~ 2021.08.19
- 공공기관 홈페이지 Contents Management System 유지보수 및 기능개선
- 스펙
  - BE : Java 1.7, Spring 3.9, iBatis, mariaDB, oracle 11g, Cubrid, Freemarker 2.3, Apache Tiles, Facebook SDK
  - FE : jQuery 1.1
  - INFRA : Tomcat 7, Apache httpd 2.4.4, Linux Ubuntu

#### 부천 여성청소년 재단 강의/대관 기능 개선

- 2021.05.01 ~ 2021.05.30
- 시설대관/교육프로그램 예약 시스템 기능 개선
- 온라인 강의 출석체크/수료증발급 기능 개발
- SNS(Facebook, Instagram) 게시물 연동 기능 개발

#### 하남시청 기능 개선 및 유지보수

- 2021.01.07 ~ 2021.04.31
- 2021.06.01 ~ 2021.08.19
- OS상에서 WAS 프로세스가 빈번하게 다운되는 현상 개선
  - OS shell script와 스케쥴러를 이용하여 프로세스 작동 여부 판단, 자동 재시작 기능
  - JVM GC 튜닝으로 해결
- 쳬육시설 등 부대시설 예약기능 개선
- 민원 게시판 기능개선
  - 자동화 공격 방지
  - 도배성 게시물 방지를 위한 UX 개선
- 보안취약점 개선
  - Tabnabbing
  - 서버경로 노출 취약점
  - HTTP Content-Security-Policy 헤더 누락
  - HTTP X-XSS-Protection 헤더 누락
  - HTML 중요 주석 정보 노출 취약점
  - 개인정보 (E-Mail) 유출 취약점
  - 클라이언트측(JavaScript) 쿠키 참조
  - 내부 네트워크 IP 정보 유출 가능 취약점
  - 취약한 SSL/TLS 버전 사용 취약점
  - XSS
  - 관리자 페이지 노출
  - 세션관리 미흡
- 조직도 자동 생성 기능
- 고시공고/나라장터/수의계약 API 연결
- 날씨 API 연결
- 모바일투표 기능 개선
  - 투표결과 집계 및 참여자 정보 통계
  - chart.js

#### 광명시청 평생교육, 학습동아리 사이트 개편

- 2020.12.01 ~ 2020.12.30
- 강의/강사관리, 이미지 게시판, 일정 관리기능 개발

#### 연천군청 온라인 관광책자 기능개발

- 2020.11.02 ~ 2020.11.30
- 관광지 상세정보 관리 및 지도 기능개발
- 환율/날씨정보 고시
- 공공 API, 카카오 지도 API

---

### 지엠티

#### 해양환경 오염방제 시스템 기능 개선 및 유지보수

- 2020.05 ~ 2020.10
- 사용자 로그인 기능 및 권한관리 기능 개발
  - 공인인증서 로그인 방식 제거
  - Interceptor에서 사용자 권한에 따른 접근 제어
- 가독성 떨어지는 다중 분기처리 구문의 리펙토링
- 파편화된 공통로직 일원화
- 도메인에 따른 패키지 분리
- 보안취약점 개선
- 스펙
  - BE : Spring 3.5, Java 1.8, Tibero
  - FE : JavaScript, jQeury 1.1
  - INFRA : Jboss, Apache HTTPD, Linux Ubuntu

#### 선박 자동식별시스템 데이터 분석을 위한 DB 설계

- 2020.05
- 전국 44개의 기지국에서 수집한 하루 평균 100만 건의 선박 위치정보의 5년치 텍스트 데이터를 분석 전 DB에 저장하기 위한 설계
- 스펙
  - PostgreSQL

#### 해양환경공단 골재채취선박 및 해양환경 관제 시스템

- 2019.10 ~ 2020.04
- FE : 해양 지도 개발 - Vanilla JavaScript Single Page Application
- BE : 업무 시스템/지리정보 API 개발
- 지도상에서 지점/경로/영역 생성/관리
- 폴링방식 실시간 선박위치 추적
- 폴링방식 실시간 알림 서비스
- 스펙
  - BE : Java 1.8, Spring 4.2, PostgreSQL
  - FE : OpenLayers 6.0, JavaScript (ES5), HandleBar.js, jQuery 3.1
  - INFRA : GeoServer, Tomcat 8, Apache HTTPD

#### 해양 정보 메세지 크롤러 개발

- 2019.10 ~ 2019.11
- JSON 및 HTML 데이터 수집
  - 아시아/태평양 주요 3국의 해상 정보 메세지를 스케쥴러로 수집하는 모듈 개발
- 스펙
  - Quartz, JSOUP, GSON, Java 1.8, Spring 4.2

#### 해양산업기술 컨퍼런스 포털 개발

- 2019.05 ~ 2019.09
- 컨퍼런스 참가 등록, 결제 기능
  - 이니페이, 페이팔 결제모듈 연결
- 컨퍼런스 자료 게시판
- 스펙
  - BE : INIPay, Paypal SDK, Apache Common-Email, CK Editor, Java 1.8, Spring 4.2
  - FE : jQuery 1.1
  - INFRA : Linux Ubuntu
  
---
  

## 학력

- 한국방송통신대학교
  - 컴퓨터과학과
  - 2020.03.02 ~ 2022.08.24
  - 3.6 / 4.5
  - 131 / 130
- 백제예술대학
  - 음악과
  - 2012.03.02 ~ 2017.02.28
  - 3.69 / 4.5
- 영등포고등학교 졸업
  - 문과
  - 2008.03.02 ~ 2011.02.28

## 교육 수료

- bit camp 자바기반 웹 전문 개발 과정
- 2018.06.26 ~ 2018.12.18
- Java, Oracle DB, Maria DB, HTML, CSS, Javascript, jQuery, SPRING, JSP, AJAX 등

## 병역

- 공익 이병 소집 해제
- 2014.04.01 ~ 2016.03.31

## 자격증

- SQLD
  - 한국데이터베이스진흥원
  - 취득 2022.06.24
  - 취득 번호 SQLD-045007371


```
  구체적 수치
  원티드 자소서 컨설팅
```