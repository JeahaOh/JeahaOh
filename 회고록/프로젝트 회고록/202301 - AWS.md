# AWS 전환 (S3, Cloud Front, Jenkins 배포)

인프라를 AWS로 전환하는 프로젝트에서 다음과 같은 파트를 담당하게 되었습니다.
- 수기 배포에서 Jenkins를 활용한 배포 자동화 전환.
- IDC CDN 서비스에서 AWS Cloud Front로 전환.
- 파일 관리를 OS File System에서 AWS S3로 전환.
- Spring Framework와 Redis를 연동하여 Session Clustering 구성.

이전의 배포는 다음과 같은 절차로 진행되었습니다.
1. 배포 담당자가 이클립스에서 프로젝트를 빌드
2. WEB 서버 종료
3. ftp로 WAS 서버에 파일 덮어쓰기
4. WAS 재시작
5. WEB 서버 재시작
6. 4대의 서버에 2~5번 과정 반복

해당 과정을 통해 배포할 경우 휴먼 에러가 발생하는 경우와 사용자의 Session이 끊기는 불편한 UX의 문제가 있었습니다. 이를 개선하기 위해 저는 Jenkins로 Build 셋팅을 하였습니다. 빌드 후 static 파일을 S3의 public bucket에 전송하여 Cloud Front로 delivery 할 수 있도록 설정하였습니다. 해당 개선으로 1시간 이상 소요되던 배포 작업을 버튼 한번 클릭으로 10분 이내에 종료되도록 개선했습니다.  
또한 배포 중 세션이 끊기는 문제를 해결하기 위해 AWS ElastiCache의 Redis를 Session Clustering으로 구성하여 UX를 개선했습니다.  
관리자 페이지와 사용자가 작성하는 상품 후기 이미지 등의 첨부 파일 또한 OS File System에서 AWS S3 SDK를 이용하여 S3에 저장, Cloud Front를 이용하도록 구성했습니다. 이 과정에서 절차 지향적으로 작성되어 파편화된 파일 관리 소스를 파일관리 클래스로 분리하여 공통 클래스로 리팩토링하여 유지보수성을 향상했습니다.