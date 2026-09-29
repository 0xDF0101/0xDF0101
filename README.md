<div align="center">

<img src="banner.svg" width="100%" alt="Kim Yujin — Backend Engineer" />

하나의 트랜잭션으로 묶을 수 없는 작업을 **신뢰할 수 있게** 만들고,<br/>
클라이언트 값을 **그대로 믿지 않는** 서버 경계를 고민합니다.

<a href="https://app.notion.com/p/3eaf909aa8e680809551f61c06e1f211"><img src="https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=notion&logoColor=white" /></a> <a href="https://velog.io/@path__find_er"><img src="https://img.shields.io/badge/Blog-20C997?style=for-the-badge&logo=velog&logoColor=white" /></a> <a href="mailto:u7genie@gmail.com"><img src="https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white" /></a>

</div>

현재 **NHN Academy AIoT 과정 TA** (2026.01 ~ ) — 교육생 Java · Spring · DB 실습 질의 대응, 팀 프로젝트 설계 조언

---

## Projects

### [Daiso Book Shop](https://github.com/nhnacademy-be12-daiso/Order-Payment) &nbsp;—&nbsp; MSA 온라인 서점 · 주문 도메인

<img src="https://img.shields.io/badge/%ED%8C%80%207%EC%9D%B8-555555?style=flat-square" /> <img src="https://img.shields.io/badge/2025.11%20~%202026.01%20·%202026.06%20%EA%B0%9C%EC%9D%B8%20%EB%B3%B4%EC%99%84-8a8a8a?style=flat-square" /> <a href="https://www.daiso-book.shop/"><img src="https://img.shields.io/badge/www.daiso--book.shop-2c4a63?style=flat-square&logo=googlechrome&logoColor=white" /></a>

서비스별로 DB가 분리된 환경에서 재고 · 포인트 · 쿠폰 · 주문 저장을 함께 확정해야 했습니다.<br/>
**Saga Orchestration**으로 단계를 Enum 상태머신에 캡슐화하고, **Transactional Outbox**로 커밋 후 메시지 유실을,<br/>
**eventId 기반 Dedup 로그**로 중복 수신을 막았습니다. 보상 Saga가 무한루프에 빠지던 장애의 원인을 규명해 수정했습니다.

<img src="https://img.shields.io/badge/Java%2021-007396?style=flat-square&logo=openjdk&logoColor=white" /> <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white" /> <img src="https://img.shields.io/badge/Spring%20Cloud-6DB33F?style=flat-square&logo=spring&logoColor=white" /> <img src="https://img.shields.io/badge/RabbitMQ-FF6600?style=flat-square&logo=rabbitmq&logoColor=white" /> <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" /> <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" />

### [NHN Academy 회의실 예약](https://github.com/nhn-academy-workspace/workspace-backend) &nbsp;—&nbsp; 사내 실사용

<img src="https://img.shields.io/badge/2%EC%9D%B8%20·%20%EB%B0%B1%EC%97%94%EB%93%9C%20%EC%A0%84%EB%B0%98-555555?style=flat-square" /> <img src="https://img.shields.io/badge/2026.07%20~%202026.08-8a8a8a?style=flat-square" /> <a href="https://nhn.roomly.site"><img src="https://img.shields.io/badge/nhn.roomly.site-2c4a63?style=flat-square&logo=googlechrome&logoColor=white" /></a>

TA로 일하며 회의실 사용 여부를 매번 구두로 확인해야 하는 불편을 직접 겪고 만들었습니다.<br/>
공정성 규칙(15분 단위 · 1회 2시간 · 팀당 하루 4시간)을 **10단계 검증 체인**으로 강제하고,<br/>
회의실 · TA Lock · 참여자 일정을 **3중으로 겹침 판정**했습니다.<br/>
교육생 45명 · TA 3명이 약 2개월간 사용했고, 문의 → 당일 수정 → 익일 배포로 운영했습니다.

<img src="https://img.shields.io/badge/Java%2021-007396?style=flat-square&logo=openjdk&logoColor=white" /> <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white" /> <img src="https://img.shields.io/badge/Spring%20Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white" /> <img src="https://img.shields.io/badge/JPA-59666C?style=flat-square&logo=hibernate&logoColor=white" /> <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" /> <img src="https://img.shields.io/badge/Telegram%20Bot-26A5E4?style=flat-square&logo=telegram&logoColor=white" />

### custom019 &nbsp;—&nbsp; 커스텀 의류 커스터마이저 (외주 · 1인 개발)

<img src="https://img.shields.io/badge/%EC%9A%94%EA%B5%AC%EC%82%AC%ED%95%AD%20%ED%98%91%EC%9D%98%20~%20%EC%9A%B4%EC%98%81-555555?style=flat-square" /> <img src="https://img.shields.io/badge/2026.06%20~%20%EC%A7%84%ED%96%89%20%EC%A4%91-8a8a8a?style=flat-square" /> <img src="https://img.shields.io/badge/%EB%B9%84%EA%B3%B5%EA%B0%9C%20%EC%A0%80%EC%9E%A5%EC%86%8C-6e7781?style=flat-square&logo=github&logoColor=white" />

실제 업체 의뢰를 받아 요구사항 협의부터 데이터 모델 · API · 배포 환경까지 단독으로 설계·구현했습니다.<br/>
가격 변경이 과거 주문에 소급되지 않도록 **제품 정의 / 디자인 / 동결 3층 스키마**를 설계해 주문 시점 값을 복사하고,<br/>
결제 조작을 막기 위해 금액을 클라이언트에서 받지 않고 **견적 · 주문 · 결제가 단일 계산기를 공유**하도록 했습니다.

<img src="https://img.shields.io/badge/Spring%20Boot%204-6DB33F?style=flat-square&logo=springboot&logoColor=white" /> <img src="https://img.shields.io/badge/JPA-59666C?style=flat-square&logo=hibernate&logoColor=white" /> <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" /> <img src="https://img.shields.io/badge/Flyway-CC0200?style=flat-square&logo=flyway&logoColor=white" /> <img src="https://img.shields.io/badge/MinIO-C72E49?style=flat-square&logo=minio&logoColor=white" /> <img src="https://img.shields.io/badge/%ED%86%A0%EC%8A%A4%ED%8E%98%EC%9D%B4%EB%A8%BC%EC%B8%A0-0064FF?style=flat-square" /> <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" /> <img src="https://img.shields.io/badge/Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white" />

> 설계 과정과 트레이드오프는 **[포트폴리오](https://app.notion.com/p/3eaf909aa8e680809551f61c06e1f211)** 에 정리해두었습니다.

---

## Tech Stack

| Category | Stacks |
|:---:|---|
| **Backend** | <img src="https://img.shields.io/badge/Java%2021-007396?style=for-the-badge&logo=openjdk&logoColor=white" /> <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white" /> <img src="https://img.shields.io/badge/Spring%20Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white" /> <img src="https://img.shields.io/badge/Spring%20Data%20JPA-6DB33F?style=for-the-badge&logo=spring&logoColor=white" /> <img src="https://img.shields.io/badge/Spring%20Cloud-6DB33F?style=for-the-badge&logo=spring&logoColor=white" /> |
| **Data & Messaging** | <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" /> <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" /> <img src="https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white" /> <img src="https://img.shields.io/badge/Flyway-CC0200?style=for-the-badge&logo=flyway&logoColor=white" /> <img src="https://img.shields.io/badge/MinIO-C72E49?style=for-the-badge&logo=minio&logoColor=white" /> |
| **Infra & DevOps** | <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" /> <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" /> <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" /> <img src="https://img.shields.io/badge/GHCR-181717?style=for-the-badge&logo=github&logoColor=white" /> <img src="https://img.shields.io/badge/Cloudflare-F38020?style=for-the-badge&logo=cloudflare&logoColor=white" /> |
