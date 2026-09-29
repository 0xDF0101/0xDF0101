# 김유진 · Backend Engineer

하나의 트랜잭션으로 묶을 수 없는 작업을 신뢰할 수 있게 만들고,
클라이언트 값을 그대로 믿지 않는 서버 경계를 고민합니다.

**[포트폴리오](https://app.notion.com/p/3eaf909aa8e680809551f61c06e1f211)** · [블로그](https://velog.io/@path__find_er) · u7genie@gmail.com

현재 **NHN Academy AIoT 과정 TA** (2026.01 ~ ) — 교육생 Java · Spring · DB 실습 질의 대응, 팀 프로젝트 설계 조언

---

## Projects

### [Daiso Book Shop](https://github.com/nhnacademy-be12-daiso/Order-Payment) — MSA 온라인 서점 · 주문 도메인

`팀 7인` `2025.11 ~ 2026.01 · 2026.06 개인 보완` · [www.daiso-book.shop](https://www.daiso-book.shop/)

서비스별로 DB가 분리된 환경에서 재고 · 포인트 · 쿠폰 · 주문 저장을 함께 확정해야 했습니다.
**Saga Orchestration**으로 단계를 Enum 상태머신에 캡슐화하고, **Transactional Outbox**로 커밋 후 메시지 유실을,
**eventId 기반 Dedup 로그**로 중복 수신을 막았습니다. 보상 Saga가 무한루프에 빠지던 장애의 원인을 규명해 수정했습니다.

`Java 21` `Spring Boot` `Spring Cloud` `RabbitMQ` `Redis` `MySQL`

### [NHN Academy 회의실 예약](https://github.com/nhn-academy-workspace/workspace-backend) — 사내 실사용

`2인 · 백엔드 전반` `2026.07 ~ 2026.08` · [nhn.roomly.site](https://nhn.roomly.site)

TA로 일하며 회의실 사용 여부를 매번 구두로 확인해야 하는 불편을 직접 겪고 만들었습니다.
공정성 규칙(15분 단위 · 1회 2시간 · 팀당 하루 4시간)을 **10단계 검증 체인**으로 강제하고,
회의실 · TA Lock · 참여자 일정을 **3중으로 겹침 판정**했습니다.
교육생 45명 · TA 3명이 약 2개월간 사용했고, 문의 → 당일 수정 → 익일 배포로 운영했습니다.

`Java 21` `Spring Boot` `Spring Security` `JPA` `MySQL` `Telegram Bot API`

### custom019 — 커스텀 의류 커스터마이저 (외주 · 1인 개발)

`요구사항 협의 ~ 운영` `2026.06 ~ 진행 중` · 비공개 저장소

실제 업체 의뢰를 받아 요구사항 협의부터 데이터 모델 · API · 배포 환경까지 단독으로 설계·구현했습니다.
가격 변경이 과거 주문에 소급되지 않도록 **제품 정의 / 디자인 / 동결 3층 스키마**를 설계해 주문 시점 값을 복사하고,
결제 조작을 막기 위해 금액을 클라이언트에서 받지 않고 **견적 · 주문 · 결제가 단일 계산기를 공유**하도록 했습니다.

`Spring Boot 4` `JPA` `MySQL` `Flyway` `MinIO/S3` `토스페이먼츠` `Docker` `Cloudflare`

> 설계 과정과 트레이드오프는 **[포트폴리오](https://app.notion.com/p/3eaf909aa8e680809551f61c06e1f211)** 에 정리해두었습니다.

---

## Skills

**Backend** &nbsp; Java 21 · Spring Boot · Spring Security · Spring Data JPA · Spring Cloud

**Data & Messaging** &nbsp; MySQL · Redis · RabbitMQ · Flyway · MinIO/S3

**Infra & DevOps** &nbsp; Docker · Linux · GitHub Actions · GHCR · Cloudflare
