# 눈치 (Noonchi)

한국어 코치 앱 — 상황에 맞는 한국어 표현과 롤플레이 대화를 통해 눈치(사회적 맥락 이해)를 학습하는 서비스입니다.

> ⚠️ 프로젝트 방향은 변경될 수 있습니다.

## 📦 Repositories

| 레포 | 공개 여부 | 스택 | 설명 |
|------|-----------|------|------|
| [Noonchi-FE](https://github.com/Noonchi-ai/Noonchi-FE) | Public | TypeScript | 웹 프론트엔드 |
| [Noonchi-App](https://github.com/Noonchi-ai/Noonchi-App) | Private | Dart | 모바일 앱 |
| [Noonchi-BE](https://github.com/Noonchi-ai/Noonchi-BE) | Private | Python | 백엔드 서버 (noonchi-server) |
| [Noonchi-AI](https://github.com/Noonchi-ai/Noonchi-AI) | Private | Python | AI 서버 (ASK 코칭, Roleplay 로직) |

## 🚀 시작하기

각 레포를 클론해서 로컬에 세팅하세요.

```bash
git clone https://github.com/Noonchi-ai/Noonchi-FE.git
git clone https://github.com/Noonchi-ai/Noonchi-App.git
git clone https://github.com/Noonchi-ai/Noonchi-BE.git
git clone https://github.com/Noonchi-ai/Noonchi-AI.git
```

각 레포 실행 방법은 레포별 README 참고.

### 환경 변수 (.env)

`.env` 파일은 보안상 레포에 포함되어 있지 않습니다. **Jinsung**에게 요청해서 전달받으세요.

## 🔗 Console Links

| 구분 | 서비스 | 링크 | 설명 |
|------|--------|------|------|
| 팀 협업 | Notion | [바로가기](https://app.notion.com/p/Noonchi-Team-Space-Home-23e07adbce2d809d937bc1a1d4d4c556) | 눈치 팀 노션 스페이스 |
| API 문서 | Swagger (FastAPI/OpenAPI) | [바로가기](https://noonchi-server-y3leekofpa-du.a.run.app/docs) | 눈치 서버 API 명세서. Cloud Run에 배포된 백엔드의 엔드포인트, 요청/응답 스키마를 실시간으로 확인 가능 |
| 사용자 분석 | Google Analytics 4 | [바로가기](https://analytics.google.com/analytics/web/?authuser=1#/a386060750p526526890/reports/intelligenthome?params=_u..nav%3Dmaui) | 앱 사용자 트래픽, 이벤트, 리텐션 등 행동 데이터 분석 대시보드 |
| 검색 노출 관리 | Google Search Console | [바로가기](https://search.google.com/u/1/search-console?resource_id=https%3A%2F%2Fnoonchi.ai.kr%2F&hl=ko) | noonchi.ai.kr 도메인의 검색 노출, 색인 상태, 크롤링 오류 등 SEO 관리 |

## ☁️ Infra & Cost

| 항목 | 서비스 | 결제처 |
|------|--------|--------|
| 서버 호스팅 | Google Cloud Run | GCP |
| 파일 저장소 | Google Cloud Storage | GCP |
| DB | PostgreSQL | GCP (또는 자체 호스팅) |
| 캐시 | Upstash Redis | Upstash |
| AI 대화 로직 | noonchi-ai (자체) | - |
| 음성 (TTS/STT) | Google TTS, CLOVA Speech | GCP / NCP |
| 번역 | Papago | NCP |
| 로그인 | Google OAuth2 | GCP |

## 🤖 Development AI Tools

| 도구 | 용도 | 추천 구독 | 비고 |
|------|------|-----------|------|
| **Claude** (Anthropic) | 코드 리뷰, 아키텍처 설계, 리팩토링, 문서화 | Pro 또는 Max | 긴 컨텍스트, 복잡한 로직 이해에 강점. Claude Code로 터미널/IDE 연동 가능 |
| **Codex (GPT-5.6)** | 코드 자동완성, 빠른 스니펫 생성, 반복 작업 | ChatGPT Plus/Team | 빠른 응답 속도, 짧은 작업에 적합 |
| **GitHub Copilot** | 인라인 코드 자동완성 (IDE 내) | Individual 또는 Business | 실시간 타이핑 보조용, 팀 단위면 Business 권장 |

### 추천 조합

- **설계/리뷰용**: Claude (복잡한 컨텍스트, 멀티파일 이해)
- **타이핑 보조용**: Copilot 또는 Codex (빠른 자동완성)
- **팀 단위 사용 시**: Claude Max + Copilot Business 조합이 비용 대비 효율적

> 팀 전체가 같은 도구를 쓸 경우 개인 구독보다 **Team/Business 플랜**이 관리(권한, 결제 통합) 측면에서 유리합니다.

## 흐름도

<img width="479" height="314" alt="image" src="https://github.com/user-attachments/assets/1db705cc-bdb3-4520-838f-32b1cbc76a93" />
