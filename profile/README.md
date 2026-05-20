# SKN26 4th 1st Team - 육뚝이들

> **LG Home** — 자연어로 LG 가전을 검색·추천하고, 사용설명서 기반 Q&A까지 제공하는 AI 가전 상담 서비스

`4th_project`는 Django 기반 웹 애플리케이션과 LangGraph 기반 LG봇(LGneer), Pinecone RAG를 결합해
**TV · 냉장고 · 세탁기 · 에어컨 · 청소기** 5개 카테고리에 대한 검색·추천·설명서 Q&A를 하나의 서비스 흐름으로 제공합니다.

---

## 👥 Team
<table>
  <tr>
    <td align="center">
      <img src="https://github.com/gieun-Park.png" width="110px;" /><br />
      <b>박기은</b><br />
    </td>
    <td align="center">
      <img src="https://github.com/minhyeok328.png" width="110px;" /><br />
      <b>서민혁</b><br />
    </td>
    <td align="center">
      <img src="https://github.com/Ocean-2930.png" width="110px;" /><br />
      <b>유동현</b><br />
    </td>
    <td align="center">
      <img src="https://github.com/dimolto3.png" width="110px;" /><br />
      <b>윤정연</b><br />
    </td>
    <td align="center">
      <img src="https://github.com/leere2424.png" width="110px;" /><br />
      <b>이레</b><br />
    </td>
    <td align="center">
      <img src="https://github.com/wjdduddlf112.png" width="110px;" /><br />
      <b>정영일</b><br />
    </td>
  </tr>

  <tr>
    <td align="center"><a href="https://github.com/gieun-Park"><img src="https://img.shields.io/badge/gieun-Park-34495e?style=flat&logo=github&logoColor=white"></a></td>
    <td align="center"><a href="https://github.com/minhyeok328"><img src="https://img.shields.io/badge/minhyeok328-34495e?style=flat&logo=github&logoColor=white"></a></td>
    <td align="center"><a href="https://github.com/Ocean-2930"><img src="https://img.shields.io/badge/Ocean-2930-34495e?style=flat&logo=github&logoColor=white"></a></td>
    <td align="center"><a href="https://github.com/dimolto3"><img src="https://img.shields.io/badge/dimolto3-34495e?style=flat&logo=github&logoColor=white"></a></td>
    <td align="center"><a href="https://github.com/leere2424"><img src="https://img.shields.io/badge/leere2424-34495e?style=flat&logo=github&logoColor=white"></a></td>
    <td align="center"><a href="https://github.com/wjdduddlf112"><img src="https://img.shields.io/badge/wjdduddlf112-34495e?style=flat&logo=github&logoColor=white"></a></td>
  </tr>

</table>

---

## 🛠 Tech Stack

| 영역 | 기술 |
|------|------|
| **Language** | Python 3.12+ |
| **Web** | Django 6.0, Django Templates (SSR), Tailwind CSS v4, django-tailwind, 바닐라 JS |
| **Build** | Node.js / npm (`theme/static_src` Tailwind 빌드) |
| **AI** | LangGraph, LangChain Core, OpenAI (`gpt-4o-mini`, `text-embedding-3-small`) |
| **Vector DB** | Pinecone (`user_manual` namespace) |
| **Data** | Selenium · BeautifulSoup 크롤링, Jupyter 적재, SQLite (개발), Django ORM |
| **Config** | python-dotenv (`.env`) |

---

## ✨ 주요 기능

| 구분 | 기능 |
|------|------|
| 메인 | 5개 카테고리 탐색 · LG봇 CTA |
| 검색 | 카테고리별 스펙 필터 · 가격 범위 · 페이지네이션(12건/페이지) |
| 상품 | 상세 페이지 · 찜하기 · 매뉴얼 링크 |
| 채팅 | LG봇(LGneer) — LangGraph 대화 · 히스토리 · 추천 질문 |
| 계정 | 회원가입·로그인 · 마이페이지 · 찜 목록 |
| AI | fall case 거절 · 후속 질문 · 찜 범위(`from_favorites`) 검색 |

---

## 📚 Docs Hub

`4th_project`는 루트 README 외에 구현·운영 중심의 기술 위키를 `docs/`로 분리해 관리합니다.

| 구분 | 링크 |
|------|------|
| Project README | [4th_project README](https://github.com/SKN26-4th-1st/4th_project/blob/main/README.md) |
| Docs Index | [docs/README.md](https://github.com/SKN26-4th-1st/4th_project/blob/main/docs/README.md) |
| Project Overview | [docs/00-overview/project-overview.md](https://github.com/SKN26-4th-1st/4th_project/blob/main/docs/00-overview/project-overview.md) |
| Getting Started | [docs/01-getting-started/development-environment.md](https://github.com/SKN26-4th-1st/4th_project/blob/main/docs/01-getting-started/development-environment.md) |
| Architecture | [docs/02-architecture/system-architecture.md](https://github.com/SKN26-4th-1st/4th_project/blob/main/docs/02-architecture/system-architecture.md) |
| Directory | [docs/02-architecture/directory-structure.md](https://github.com/SKN26-4th-1st/4th_project/blob/main/docs/02-architecture/directory-structure.md) |
| Data Pipeline | [docs/02-architecture/data-pipeline.md](https://github.com/SKN26-4th-1st/4th_project/blob/main/docs/02-architecture/data-pipeline.md) |
| DB Schema | [docs/05-database/schema-and-erd.md](https://github.com/SKN26-4th-1st/4th_project/blob/main/docs/05-database/schema-and-erd.md) |
| API | [docs/06-api/rest-api.md](https://github.com/SKN26-4th-1st/4th_project/blob/main/docs/06-api/rest-api.md) |
| LangGraph | [docs/07-ai-modeling/langgraph-flow.md](https://github.com/SKN26-4th-1st/4th_project/blob/main/docs/07-ai-modeling/langgraph-flow.md) |
| RAG · Pinecone | [docs/07-ai-modeling/rag-pinecone.md](https://github.com/SKN26-4th-1st/4th_project/blob/main/docs/07-ai-modeling/rag-pinecone.md) |
| Features | [docs/08-features/README.md](https://github.com/SKN26-4th-1st/4th_project/blob/main/docs/08-features/README.md) |
| Frontend | [docs/03-frontend/README.md](https://github.com/SKN26-4th-1st/4th_project/blob/main/docs/03-frontend/README.md) |

---

## Team Identity

복잡한 가전 스펙표와 긴 사용설명서 사이에서 사용자가 **원하는 조건을 말로 전달**하고, **근거 있는 추천·안내**를 받을 수 있게 만드는 것을 목표로 합니다.

- **LG봇(LGneer)**: 자연어 질의 → 제품군 분류(TVT/ACT/REF/VAC/WMT) → 조건 추출 → DB 검색 + 매뉴얼 RAG → 답변 생성
- **LG Home UI**: 카테고리별 필터 검색, 상품 상세, 찜(관심 제품), 대화형 추천

---

## Core Capabilities

| 역할 | 담당 영역 |
|------|-----------|
| **Frontend** (박기은, 서민혁) | Figma 화면 설계, Django SSR·컴포넌트, Tailwind UI, 검색/채팅/마이페이지·`api-response.js` 등 클라이언트 연동 |
| **Backend** (유동현) | Django URL·뷰·API(`send_chat`, 찜), 인증, ORM 검색·채팅 DB 연동, LangGraph 실행 연결 |
| **Modeling · RAG** (윤정연) | 사용설명서 PDF 전처리·청킹, Pinecone 적재·메타데이터, 요구사항 정의 |
| **Modeling · Agent** (정영일) | LangGraph 노드·분기 설계, `llm_agent.py` 프롬프트·structured output, fall case·후속 질문 라우팅 |
| **Database** (이레) | LG 공식몰 크롤링·전처리, 카테고리별 `Product*` 스키마 적재, 데이터 품질·평가 기록 |

공통으로 **Git 기반 협업**(PR / Issue / Conventional Commits)과 **프롬프트·RAG·평가 근거 문서화**를 지향합니다.

---

## Working Method

- Issue 기반 작업 분리
- Branch 전략 준수
- Conventional Commit 사용
- PR 리뷰 후 Merge
- 프롬프트·RAG 설정·평가 결과 및 설계 근거 문서화 (`README` + `docs`)

---

## Repository Philosophy

각 프로젝트는 독립된 저장소로 관리하며, 다음 원칙을 따릅니다.

- 구조화된 폴더 구성 (`config`, `accounts`, `products`, `chats`, `api`, `common`, `mainpage`, `templates`, `static`, `theme`, `docs` 등)
- 데이터·문서·비밀값(`.env`) 분리 관리
- 설정·의존성·평가 항목 버전 관리
- 산출물 및 실험 기록 유지

---

## 📂 Main Repository

| 저장소 | 설명 |
|--------|------|
| [4th_project](https://github.com/SKN26-4th-1st/4th_project) | LG Home 웹 애플리케이션 및 LLM 파이프라인 |
