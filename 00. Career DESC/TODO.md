
---
  
## repository 정리 방향

- 이력서, 경력기술서, 자소서로 분리 및 전체 기록 통합
  - 이력서
    - 자기소개 요약
    - 강점
    - 사용 가능 기술
    - 연락처
    - 재직 경력 및 주요성과 요약
  - 경력기술서
    - 프로젝트 별 요약
    - 전체 경력과 지원용 요약 경력 정리
    - 성과 중심 프로젝트 정리
  - 자소서
    - 젼체 이력서 (프로젝트별 컬쳐 핏 관점, 인성 관점, 기술 관점으로 분리)
- 지원 회사별 자소서 문항 모음
- 지원 할만한 회사 JD 모음
  - 향후 이직용 keyword 정리용
- 면접 대비 질문 정리 (ready for tech interview)
  - 기술
  - 인성
  - 컬쳐 핏

## 면접 대비 준비할 기초 지식

- NoSQL
  - Redis
  - Memcahced
  - MongoDB
- Transactional
  - 동작 원리
    - Proxy 방식으로 동작.
    - AOP Proxy가 기존 코드를 가로채서 앞 뒤로 transaction 처리를 할 수 있는 코드를 배치해서 하나의 TX로 처리될 수 있는 것.
  - Propagation
    - REQUIRED
    - SUPPORTS
    - MANDATORY
    - NEVER
    - NOT_SUPPORTED
    - REQUIRES_NEW
    - NESTED
  - TX의 격리 레벨 (Isolation)
    - DEFAULT
    - READ_UNCOMMITTED
    - READ_COMMITTED
    - REPEATABLE_READ
    - SERIALIZABLE
    - MVCC
  - readOnly
    - transaction의 FlushMode를 NEVER로 설정, flush를 사용하지 않으면 비용이 절감, 생성/수정/삭제가 일어나지 않기 때문에 성능상 이점 발생.
  - rollbackFor
  - timeout
- checked exception, unchecked exception

---