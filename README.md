<h1 align="center">김상우</h1>

<p align="center">
  <b>백엔드 개발자</b> · Java / Spring Boot<br/>
  <sub>만든 것이 실제로 맞게 동작하는지, 로그와 수치로 직접 확인합니다.</sub>
</p>

<table align="center">
  <tr>
    <td align="center" width="25%"><h2>207 → 18ms</h2><sub><b>시세 API 평균 응답</b><br/>캐시 적용 · 운영 서버 JMeter 실측</sub></td>
    <td align="center" width="25%"><h2>480 → 5.8ms</h2><sub><b>메타덱 조회 N+1 개선</b><br/>쿼리 로그로 진단 · 로컬 JMeter</sub></td>
    <td align="center" width="25%"><h2>PR 120건</h2><sub><b>96% Claude Code 흔적 · 79% 사람 리뷰</b><br/>GitHub API로 직접 감사</sub></td>
    <td align="center" width="25%"><h2>버그 2건</h2><sub><b>LLM 자동 채점이 찾은 실제 버그</b><br/>매일 자동 실행되는 피드백 에이전트</sub></td>
  </tr>
</table>

<p align="center">
  <a href="https://s4ngg.github.io"><b>포트폴리오</b></a> ·
  <a href="https://s4ngg.github.io/troubleshooting.html">트러블슈팅</a> ·
  <a href="https://s4ngg.github.io/performance.html">성능 개선</a> ·
  <a href="https://github.com/s4ngg/Lojipsa/blob/main/TROUBLESHOOTING.md">운영 중 서비스 장애 기록</a>
</p>

### 대표 프로젝트

| 프로젝트 | 무엇을 했나 | 근거 |
|---|---|---|
| **[Lojipsa](https://github.com/s4ngg/Lojipsa)**<br/><sub>로스트아크 AI 에이전트 서비스<br/>1인 기획·개발·배포·운영</sub> | Claude 요약·추천에 관리자가 편집하는 배경지식을 주입하고, 핵심 LLM 기능을 매일 채점하는 피드백 에이전트로 품질을 점검합니다.<br/>1GB 서버 배포 사고를 겪은 뒤 로컬 빌드·업로드 방식으로 절차를 바꿨습니다. | [운영 서버 실측<br/>(207→18ms, 436→37ms)](https://s4ngg.github.io/performance.html) |
| **[TFT-gogo](https://github.com/s4ngg/TFT-gogo)**<br/><sub>롤토체스 전적 검색 서비스<br/>팀장 · 풀스택 4인</sub> | 쿼리 로그로 N+1을 찾아 조회를 재설계했고, 외부 AI 호출이 묶인 트랜잭션을 나눠 응답을 429 → 355ms로 줄였습니다.<br/>pgvector 유사도 추천에 circuit breaker 폴백을 두었습니다. | [JMeter 50명·5분·3회<br/>(로컬 측정)](https://s4ngg.github.io/performance.html) |
| **[AllPick](https://github.com/s4ngg/AP-Spring)**<br/><sub>역할 기반 쇼핑몰 서비스<br/>팀장 · 풀스택 6인</sub> | 쿠폰·멤버십을 설계하고 도메인 분리와 공통 예외 응답을 정했습니다. JWT 역할별 권한과 결제 상태 추적을 구현했고, AI 추천 서버([AP-FastAPI](https://github.com/s4ngg/AP-FastAPI))는 단독으로 개발해 연동했습니다. | 백엔드 병합 PR 44건<br/>(저장소 109건 중) |
| **[portfolio-agent](https://github.com/s4ngg/portfolio-agent)**<br/><sub>포트폴리오 RAG 챗봇<br/>1인 사이드 프로젝트</sub> | 방문자 질문에 실제 프로젝트 문서만 근거로 답하도록 제한한 RAG 파이프라인입니다. | — |

### 기술 스택

**주력** &nbsp;
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring%20Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)

**함께 써본 것** &nbsp;
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=s4ngg&show_icons=true&theme=dark&hide_border=true&count_private=true" alt="s4ngg's GitHub stats" height="165" />
</p>

<p align="center">📫 s4ngg@naver.com</p>
