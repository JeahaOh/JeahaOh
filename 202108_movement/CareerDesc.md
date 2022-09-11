# 경력 기술서

## Profile

- 이름 : 오제하
- 직무 경력 :
  - 지엠티 (현직장) : 사원 2019.05.20 ~ 재직 중
  - 주식회사 미디어젠 : 인턴 2019.02.11 ~ 2019.04.11
- 블로그 : [jeaha.dev](http://jeaha.dev)
- 깃헙 : [jeahaOh](https://github.com/JeahaOh)

## Skill

- Language :  
  JAVA, JavaScript, SQL
- Framework And Library :  
  Spring, JSP, NodeJS, Express, React
- OS :  
  Mac OSX, Windows, Linux Ubuntu

---

## Project

### [2020.04. ~ 2020.10.] 해양 환경 오염 방제 시스템 기능개선 및 유지보수

- 주요 역할 및 담당 업무 : 사용자 권한 관리 및 인터셉터 단 접근 제어, 공통 함수 기능 개선, 보안취약점 개선
- 상세 업무 :
  - 공무원 유져 테이블과 외부 업체 유져 테이블을 연계하여 로그인, 권한 관리.
  - 사용자 권한에 따른 Interceptor 단에서 접근 제어.
  - 프로젝트 이전 유지보수 기간 동안 만들어진 다원화 된 공통 로직 일원화.
  - 체계없이 얽혀 있는 if-else 문 간단하게 읽힐 수 있도록 리팩토링.
  - 다중 상속 클래스 단순화.
  - 버젼 관리가 되지 않은 소스의 정상화.
  - 기능에 따른 패키지 분리.
  - 관리자 기능, 공통 엑셀 다운로드 및 화면 프린트 기능 개선.
  - 보안 취약점 개선.

---

### [2020.05] 국책 과제 AIS 데이터 분석

- 주요 역할 및 담당 업무 : DB설계
- 주제 :
  - 전국에 총 44대의 AIS 수신기가 있고, 한 기지국 당 하루 평균 100만 건의 AIS 데이터가 수집됩니다.
  - 이 데이터들은 암호화된 데이터를 복호화 후, AIS 데이터 분석 과제를 수행하게 되었습니다.
  - 저는 복호화된 데이터를 저장하기 위해 DB 설계를 하였습니다.

---

### [2020.04] 해수부 지능형 선박 관제 시스템 프로젝트 기술지원

- 주요 역할 및 담당 업무 : 선박의 사용 통신망에 따른 과거 항적 조회 기능 기술지원
- 상세 업무  
  전국에 선박들은 1대당 1일에 약 3600건의 위치와 상태 데이터를 통신망에 따라 구분하여 DB에 저장합니다. (만약, LTE망으로 수신기에 데이터를 전송해 준다면 'LTE_20200912'라는 테이블에 데이터를 저장합니다.) 이렇게 쌓인 항적 데이터를 조회하여 지도위에 표출하는 기능을 만들었습니다.

---

### [2019.10. ~ 2020.03.] 해양환경공단 골재채취선박 및 해양환경 관제 시스템

- 주제 :
- 주요 역할 : 전자 해도 제작
- 담당 업무 :
  - OpenLayers 6.0을 이용하여 HTML5에 지도 생성.
    - 관제사가 지도 위에 관리를 위한 지점/거리/영역 생성, 관리, 스타일 적용, DB에 저장 후 관제사의 업무 프로세스에 사용하도록 함.
    - 지도 위의 거리 측정.
    - 실시간 선박 위치 표출.
    - 선박 과거 항적 조회 및 표출.
    - 실시간 알림 서비스. (문자, 웹 표출)
  - GeoServer를 이용하여 PostgreSQL의 데이터 Layer 생성.
  - 두 지점 사이의 수심 변화 데이터 표출. (PostgreSQL와 PostGIS를 이용.)
  - 영역 데이터와 기준 영역 데이터 비교, 유효한지 확인하는 기능. (PostgreSQL와 PostGIS를 이용.)
  - 대량의 GIS 데이터 Client/Server Side에서 유효성 체크 후 DB 업로드.

---

### [2019.09. ~ 2019.10] APPWeb 개발

- 주제 : 아시아 오세아니아 해상 교통안전을 위한 웹 서비스 연구 개발 프로젝트
- 주요 역할 : 환태평양 주요 3국의 해상안전 메세지 수집
- 담당 업무 : 환태평양 주요 3개국에서 발행하는 해상 안전 메세지를 수집하는 모듈을 제작하였습니다. 스케쥴러로 일정한 시간 간격을 두고 요청 하여 json 형식 또는 html 형식으로 데이터를 받은 뒤, html이라면 JSOUP을 이용하여 파싱, 유효성 검사, 데이터 타입, 좌표계와 시간 등을 고려하여 데이터 전처리 후 DB에 저장하는 모듈 개발.

---

### [2019.05.28 ~ 2019.09.] E-navigation Underway Conference Portal 개발

- 주제 : 국제 해양산업기술 컨퍼런스 역대 발표자료 정리 게시판과 해수부 주최 컨퍼런스 참가 등록, 결제 모듈 연동.
- 담당 업무 :
  - INIPay 결제 모듈을 이용하여 국내 이용자 결제기능 (웹, 모바일 가능).
  - Paypal 결제 모듈을 이용하여 국외 이용자 결제기능.
  - JavaScript를 이용하여 결제자, 결제일, 결제 금액, 결제 상태 등 목록 Excel 다운로드 기능.
  - 전자정부 프레임워크를 개량하여 일반 게시판과 공지사항 게시판 관리 기능.
  - Spring Security를 이용하여 접속자 권한 관리.
  - Apache Common-Email 라이브러리를 이용하여 이용자 결제 시 결제 명세서 발송.
  - CK Editor를 이용하여 게시물 작성 시 본문 내용 HTML로 변환 저장 기능.
  - Slack API를 이용하여 프로젝트 에러 리포트 기능.
- 개발 환경 : Windows, Linux(Gabia Hosting)
- 개발 언어 및 라이브러리 :  
  INIPay(webStandard, Mobile), Paypal SDK, Apache Common-Email, CK Editor, Java 1.8, JavaScript, 전자정부 3.7, MySQL

---

### [2019.02.11 ~ 2019.04.11] YUMMY APP, WEB 개발

- 주제 : [인턴 과제 프로젝트]  
  안드로이드 어플리케이션과 스프링 웹 서버를 구현, 자율 주제로 미슐렝 가이드 레스토랑 관련 서비스 개발.
- 기능 :
  - 어플리케이션
    - 카메라 기능, Recycler View, Card View, 사진을 포함한 게시물 CRUD.
  - 웹
    - 멀티파트 사진을 포함한 게시물 CRUD.
    - 사용자의 평점을 분석하여 레스토랑 평점 통계.
- 역할 : 기획, 설계, 프로그래밍.
- 개발 환경 : Mac OS, Windows, Linux(AWS EC2).
- 개발 언어 및 라이브러리 :  
  Retrofit2, Piccasso, Google Map API,  
  Jackson, jQuery, Gson,  
  MariaDB,  
  전자정부 프레임워크 3.6, Android Espresso,  
  Java11, JavaScript 등
- 비고 :
  - 사용자의 평점을 베이지안 통계를 이용하여 분석, 레스토랑에 대한 평점을 냄.
  - 1인 개발.

---

### [2018.10.01 ~ 2018.12.17] SceneCok 개발

- 주제 : [팀 과제 프로젝트]  
  'Discover and Share a constantly expanding Movie Around The World'를 슬로건으로 기존의 영화 리뷰 웹, 영화 상영 서비스, 영화 평점 서비스와는 다르게 최신 영화만이 아닌, 'SNS 형식'과 '장면 콘텐츠'를 통해 "영화 정보 발견과 공유를 위한 플렛폼".
- 담당 업무 :
  - DB 설계
  - Kakao API를 이용하여 사용자의 가입/탈퇴/로그인 기능.
  - The MovieDB API를 이용하여 영화 데이터 표출.
  - Apache Tiles를 이용하여 레이아웃 설정.
  - 사용자의 영화 기호를 분석하여 영화를 추천해 주는 기능.
  - 사용자의 게시물 편집/삭제 기능.
  - AWS를 사용한 클라우드 서버 배포.
- 역할 : 기획, 설계, 프로그래밍.
- 개발 환경 : Mac OS, Linux(AWS EC2).
- 개발 언어 및 라이브러리 :  
  OpenJDK 11, Apache Tomcat 9.0.12, Spring Framework 5.1.1, Spring WebMVC 5.1.1, MyBatis 3.4.6, Apache Tiles 3.0.8, MariaDB, HTML 5, CSS 3, JavaScript, BootStrap 4.1.3, jQuery, AJAX, Jackson 2.9, JSP, JSTL, Eclipse 2018-09, eXERD, Brakets, Visual Studio Code, Gradle 5.0, The Movie DB API, Kakao Login API, Google Maps API, Chart.js, Starrr.js, Noty.js, AOS.js, typeahead.js, PuTTY, Z shell, AWS EC2(Linux), GitHub, Trello, slack, Google Drive, Kakao oven
- 비고 :
  - 소스코드 : https://github.com/JeahaOh/java110-team-project-1
  - 시연 영상 : https://youtu.be/rFDSViXZMn8
