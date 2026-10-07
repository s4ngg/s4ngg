### 김상우 — 백엔드 개발자

Spring Boot로 API를 만들고, 그게 실제로 맞게 동작하는지 로그와 PR 기록으로 직접 확인하는 걸 기준으로 삼습니다. AI 코딩 도구를 쓸 때도 "그럴듯한 코드"가 아니라 "실제로 맞는 코드"인지를 PR 단위로 추적해서 검증합니다.

#### 프로젝트

**[Lojipsa](https://github.com/s4ngg/Lojipsa)** · 로스트아크 AI 에이전트 서비스 · 1인 기획·개발·배포·운영
- 스케줄러로 동작하는 Slack 알림 에이전트 3종, 관리자가 편집한 배경지식을 주입해 모델이 최신 정보를 추측하지 않게 한 Claude 요약·추천
- 핵심 LLM 기능을 매일 합성 시나리오로 실행하고 Claude가 다시 PASS/FAIL로 채점하는 피드백 에이전트 — 이 방식으로 실제 버그 2건 발견(응답 첫 블록이 답변이 아닐 때의 NPE, 채점 실패를 정상으로 보고하던 문제)
- 시세 API에 데이터 성격별 TTL 캐시(재료 5분·보석 1분) 적용, **운영 서버** JMeter(1스레드·120초·3회) 평균 응답 207ms → 18ms, 436ms → 37ms
- 1GB EC2에서 Docker 빌드 중 서버가 응답 불능이 된 사고를 겪고, 로컬 빌드 후 결과물만 올리는 방식으로 배포 절차를 바꿔 문서화

**[TFT-gogo](https://github.com/s4ngg/TFT-gogo)** · 롤토체스 전적 검색 서비스 · 팀장/풀스택 4인
- 병합된 PR 120건을 GitHub API로 직접 감사해 96%에 Claude Code 흔적, 79%에 사람 리뷰가 있었음을 확인
- 메타덱 조회 N+1을 쿼리 로그로 찾아 JMeter(50명·5분·3회, 로컬)로 평균 480ms → 5.8ms
- AI 추천 API에서 DB 조회와 외부 AI 호출이 한 트랜잭션에 묶여 커넥션이 오래 점유되던 문제를 트랜잭션 범위 재설계로 평균 429ms → 355ms
- OpenAI 임베딩 + pgvector 유사도 기반 하이브리드 추천, 검색 실패 시 circuit breaker로 기존 방식 폴백

**[AllPick](https://github.com/s4ngg/AP-Spring)** · 역할 기반 쇼핑몰 서비스 · 팀장/풀스택 6인
- 쿠폰·멤버십 설계, 쿠폰 정책 변경이 주문 코드에 번지던 문제를 계기로 회원·상품·주문·쿠폰 도메인 분리와 공통 예외 응답 적용
- Spring Security + JWT 역할별(회원/판매자/관리자) 권한 분리, Toss 결제부터 환불까지 상태 추적
- AI 상품 추천 서버([AP-FastAPI](https://github.com/s4ngg/AP-FastAPI))를 FastAPI로 단독 개발해 백엔드와 연동, GitHub Actions로 배포 자동화

**[portfolio-agent](https://github.com/s4ngg/portfolio-agent)** · 포트폴리오 RAG 챗봇 · 1인 사이드 프로젝트
- 방문자 질문에 실제 프로젝트 문서만 근거로 답하도록 제한한 RAG 파이프라인

#### 기술 스택

지금 주로 쓰는 것
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring%20Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)

팀 프로젝트에서 써본 것
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

<img src="https://github-readme-stats.vercel.app/api?username=s4ngg&show_icons=true&theme=dark&hide_border=true&count_private=true" alt="s4ngg's GitHub stats" height="165" />

📫 s4ngg@naver.com · 전체 프로젝트와 PR 기록은 **[s4ngg.github.io](https://s4ngg.github.io)**에서 확인할 수 있습니다.
