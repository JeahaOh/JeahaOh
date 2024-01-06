# AboutJeaha

About Jeaha

---
면접 대비 준비할 기초 지식
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
