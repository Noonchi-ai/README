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
