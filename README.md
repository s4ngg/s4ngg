### 김상우 — 백엔드 개발자

Spring Boot로 API를 만들고, 그게 실제로 맞게 동작하는지 로그와 PR 기록으로 직접 확인하는 걸 기준으로 삼습니다. AI 코딩 도구를 쓸 때도 "그럴듯한 코드"가 아니라 "실제로 맞는 코드"인지를 PR 단위로 추적해서 검증합니다.

#### 프로젝트

| 프로젝트 | 역할 | 핵심 |
|---|---|---|
| **[Lojipsa](https://github.com/s4ngg/Lojipsa)**<br>로스트아크 AI 에이전트 서비스 | 1인 기획·개발·배포·운영 | 매일 자동 실행되는 LLM-as-judge 피드백 에이전트로 실제 버그 2건 발견<br>시세 API TTL 캐시, **운영 서버** JMeter 평균 207ms → 18ms · 436ms → 37ms<br>1GB EC2 배포 사고 후 로컬 빌드·업로드 방식으로 절차 변경 |
| **[TFT-gogo](https://github.com/s4ngg/TFT-gogo)**<br>롤토체스 전적 검색 서비스 | 팀장 · 풀스택 4인 | 병합 PR 120건 감사: 96% Claude Code 흔적, 79% 사람 리뷰<br>N+1 개선 480ms → 5.8ms (JMeter 50명·5분·3회, 로컬)<br>외부 AI 호출이 묶인 트랜잭션 재설계 429ms → 355ms, pgvector 추천 + 폴백 |
| **[AllPick](https://github.com/s4ngg/AP-Spring)**<br>역할 기반 쇼핑몰 서비스 | 팀장 · 풀스택 6인 | 쿠폰·멤버십 설계, 도메인 분리와 공통 예외 응답, JWT 역할별 권한<br>AI 추천 서버([AP-FastAPI](https://github.com/s4ngg/AP-FastAPI)) 단독 개발·연동, GitHub Actions 배포 |
| **[portfolio-agent](https://github.com/s4ngg/portfolio-agent)**<br>포트폴리오 RAG 챗봇 | 1인 사이드 프로젝트 | 실제 프로젝트 문서만 근거로 답하도록 제한한 RAG 파이프라인 |

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
