- blog-search
    - dependency : lombok
  - external-api
    - Presentation Layer (Controller, Service)
    - dependency : spring-boot-starter-web, client-core, client-kakao
  - client
    - core
      - Business Layer (Domain)
      - dependency : spring-cloud-starter-openfeign, infra-h2
    - kakao
      - api 호출 클라이언트
      - dependency : spring-cloud-starter-openfeign, infra-h2
  - infra
    - h2
      - Persistence Layer (Repository, Entity)
      - dependency : spring-boot-starter-data-jap, com.h2database
