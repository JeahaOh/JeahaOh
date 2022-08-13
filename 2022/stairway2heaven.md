## 아이디룩

자사 쇼핑몰 유지보수 및 개선
- 프로모션 기능 개선
  - 랜덤뽑기, 출석체크 등 이벤트 기능 개발
- 엑셀 업/다운로드 기능 개선
  - 스프링 - 쿼츠, POI를 이용한 정기적인 매출 데이터 데이터 추출 자동화
  - 결과 파일을 S3에 저장하여 slack으로 다운로드 링크를 포함한 알림이 가도록 함
- 코드 클리닝 및 리팩토링
  - 소스코드 내 하드코드 제거
  - 파일 경로, api key 등의 변수 property화
  - 파편화된 소스, 중복 소스, 과도한 IF문 중첩 구문 등의 리팩토링
- 트래픽 개선
  - 어플리케이션 내 정적 리소스의 AWS Cloud Front를 통해 배포
  - redis를 사용한 세션 클러스터링 구성
- 인프라 개선
  - IDC -> AWS Cloud 전환
  - 정적 리소스 서비스 및 파일 업다운로드 기능을 OS File System에서 AWS S3 API로 전환
  - tmax webtob에서 nginx로 전환
  - 커넥션타임, 압축, 헤더 설정과 whitelist 방식의 back office 접근 제어 설정
- 사용 기술
  - java 1.7, spring 3.1, myBatis, oracle 11g, tomcat 7, nginx, apache tiles, AWS EC2, S3, jenkins, code deploy, github


## 한신

공공기관 홈페이지 외주 유지보수
- 체육시설 및 대관 기능 개선
- SNS 게시물 연동 기능 개발
- 유투브 API를 이용하여 강의수강 및 출석체크 프로그램 개발
- 공공 API 연동 정보 제공 프로그램 기능개선
- 보안취약점 점검 및 개선
  - 크로스사이트 스크립트
  - 쿠키 변조
  - 데이터 평문 전송
  - 자동화 공격
  - 세션 예측
  - 불충분한 인가
- 사용 기술
  - java 1.7, spring 3.9, iBatis, mariaDB, oracle 11g, cubrid, tomcat7, apache httpd 2.4.4, freemarker 2.3, apache tiles, facebook sdk, linux server, svn ...

## GMT

해수부 하청, 해양 관련 프로젝트를 주로 진행
- WEB GIS 개발(전자해도)
  - vanilla javascript로 spa 지도를 구현 개발
  - 선박의 과거 이동 루트 추적기능 개발
- GIS 관련 rest API 개발
- 국내외 해양 지리 정보 파서 / 크롤러 개발
- 해양 컨퍼런스 예약 시스템 개발
- Interceptor를 이용한 역할 기반 권한 관리
- 진행 프로젝트
  - 해경 해양오염방제 시스템 기능개선
  - 목포해양대 AIS 데이터 분석
  - 해수부 지능형 선박관제시스템 개발
  - 해양환경관리공단 골재채취 선박 및 해양환경 관제시스템 개발
  - 해수부 Digital At Sea Web
  - 목포해양대 ENUW 컨퍼런스 홈페이지 개발
- 사용 기술
  - java 1.8, spring 4.1, iBatis, oracle 11g, postgreSQL, tomcat 8, httpd 2.4.4, apache tiles, openlayers 6, leaflet
