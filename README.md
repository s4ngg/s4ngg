# 김상우

**백엔드 개발자** — Java, Spring Boot

만든 것이 실제로 맞게 동작하는지, 로그와 수치로 확인하는 것을 기준으로 일합니다.

[포트폴리오](https://s4ngg.github.io) · [트러블슈팅](https://s4ngg.github.io/troubleshooting.html) · [성능 개선](https://s4ngg.github.io/performance.html) · [운영 장애 기록](https://github.com/s4ngg/Lojipsa/blob/main/TROUBLESHOOTING.md) · [s4ngg@naver.com](mailto:s4ngg@naver.com)

## About

- Spring Boot로 API를 설계하고, 느린 구간은 쿼리 로그와 JMeter로 원인을 확인한 뒤 고칩니다. 측정 결과에는 로컬인지 운영 서버인지 함께 적습니다.
- AI 코딩 도구를 쓰되, 결과는 PR 단위로 리뷰하고 검증합니다. 팀 프로젝트의 병합 PR 120건을 직접 감사해 96%에 Claude Code 흔적, 79%에 사람 리뷰가 있음을 확인했습니다.
- LLM 기능을 서비스에 붙일 때는 모델이 틀리거나 실패해도 서비스가 멈추지 않도록 폴백과 자동 점검을 함께 설계합니다.
- 남서울대학교 지능정보통신공학과 졸업 (2026.02)

## 주요 작업

| 프로젝트 | 내용 | 근거 |
|---|---|---|
| **[Lojipsa](https://github.com/s4ngg/Lojipsa)**<br/>로스트아크 AI 에이전트 서비스 · 1인 | Slack 알림 에이전트 3종과 Claude 요약·추천을 운영합니다. 핵심 LLM 기능을 매일 채점하는 피드백 에이전트로 실제 버그 2건을 찾았습니다. 시세 API는 TTL 캐시로 운영 서버 기준 평균 207ms → 18ms, 436ms → 37ms로 줄였습니다. | [성능 개선 기록](https://s4ngg.github.io/performance.html)<br/>[장애 기록](https://github.com/s4ngg/Lojipsa/blob/main/TROUBLESHOOTING.md) |
| **[TFT-gogo](https://github.com/s4ngg/TFT-gogo)**<br/>롤토체스 전적 검색 서비스 · 팀장, 4인 | 쿼리 로그로 N+1을 찾아 조회를 재설계해 평균 480ms → 5.8ms(로컬 JMeter)로 줄였습니다. 외부 AI 호출이 묶인 트랜잭션을 나눠 응답을 429ms → 355ms로 줄였고, pgvector 추천에는 circuit breaker 폴백을 두었습니다. | [성능 개선 기록](https://s4ngg.github.io/performance.html) |
| **[AllPick](https://github.com/s4ngg/AP-Spring)**<br/>역할 기반 쇼핑몰 서비스 · 팀장, 6인 | 쿠폰·멤버십을 설계하고 도메인 분리와 공통 예외 응답, JWT 역할별 권한을 구현했습니다. AI 추천 서버([AP-FastAPI](https://github.com/s4ngg/AP-FastAPI))는 단독으로 개발해 연동했습니다. | 백엔드 병합 PR 44건 (저장소 109건 중) |

## 기술

Java · Spring Boot · Spring Security · JPA · MySQL · PostgreSQL · Redis<br/>
Docker · AWS (EC2, ECS, RDS) · GitHub Actions · JMeter<br/>
FastAPI · TypeScript · React · Next.js
