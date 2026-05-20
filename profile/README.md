# SKN26 4th 1st Team

> **LG Home** — 자연어로 LG 가전을 검색·추천하고, 사용설명서 기반 Q&A까지 제공하는 AI 가전 상담 서비스

[SKN26 4th Project README](https://github.com/SKN26-4th-1st/4th_project/blob/main/README.md)에서 아키텍처, 설치 방법, 평가 결과를 확인할 수 있습니다.

---

## 👥 Team

<table>
  <tr>
    <td align="center">
      <img src="https://github.com/gieun-Park.png" width="110px;" /><br />
      <b>박기은</b><br />
      <sub>Frontend</sub><br />
      <a href="https://github.com/gieun-Park">@gieun-Park</a>
    </td>
    <td align="center">
      <img src="https://github.com/minhyeok328.png" width="110px;" /><br />
      <b>서민혁</b><br />
      <sub>Frontend</sub><br />
      <a href="https://github.com/minhyeok328">@minhyeok328</a>
    </td>
    <td align="center">
      <img src="https://github.com/Ocean-2930.png" width="110px;" /><br />
      <b>유동현</b><br />
      <sub>Backend</sub><br />
      <a href="https://github.com/Ocean-2930">@Ocean-2930</a>
    </td>
    <td align="center">
      <img src="https://github.com/dimolto3.png" width="110px;" /><br />
      <b>윤정연</b><br />
      <sub>Modeling</sub><br />
      <a href="https://github.com/dimolto3">@dimolto3</a>
    </td>
    <td align="center">
      <img src="https://github.com/leere2424.png" width="110px;" /><br />
      <b>이레</b><br />
      <sub>Database</sub><br />
      <a href="https://github.com/leere2424">@leere2424</a>
    </td>
    <td align="center">
      <img src="https://github.com/wjdduddlf112.png" width="110px;" /><br />
      <b>정영일</b><br />
      <sub>Modeling</sub><br />
      <a href="https://github.com/wjdduddlf112">@wjdduddlf112</a>
    </td>
  </tr>
</table>

---

## 🛠 Tech Stack

| 영역 | 기술 |
|------|------|
| **Web** | Django 6, Django Templates, Tailwind CSS v4, django-tailwind |
| **AI** | LangGraph, LangChain, OpenAI (`gpt-4o-mini`, `text-embedding-3-small`) |
| **Vector DB** | Pinecone (사용설명서 RAG) |
| **Data** | Selenium · BeautifulSoup 크롤링, SQLite |
| **Language** | Python 3.12+ |

---

## Team Identity

복잡한 가전 스펙표와 긴 사용설명서 사이에서 사용자가 **원하는 조건을 말로 전달**하고, **근거 있는 추천·안내**를 받을 수 있게 만드는 것을 목표로 합니다.

- **LG봇(LGneer)**: 자연어 질의 → 제품군 분류 → 조건 추출 → DB 검색 + 매뉴얼 RAG → 답변 생성
- **LG Home UI**: 카테고리별 필터 검색, 상품 상세, 찜(관심 제품), 대화형 추천

---

## Core Capabilities

| 역할 | 담당 영역 |
|------|-----------|
| **Frontend** (박기은, 서민혁) | SSR 페이지·컴포넌트, Tailwind UI, 검색/채팅/마이페이지 인터랙션 |
| **Backend** (유동현) | Django API·뷰, 인증, 채팅 연동, 상품 검색 로직 |
| **Modeling** (윤정연, 정영일) | LangGraph 에이전트, 프롬프트·슬롯 설계, fall case·후속 질문 라우팅 |
| **Database** (이레) | 제품 스키마·크롤링 데이터 적재, ORM 검색, Pinecone 매뉴얼 인덱싱 |

공통으로 **Git 기반 협업**(PR / Issue / Conventional Commits)과 **프롬프트·RAG·평가 근거 문서화**를 지향합니다.

---

## Working Method

- Issue 기반 작업 분리
- Branch 전략 준수
- Conventional Commit 사용
- PR 리뷰 후 Merge
- 프롬프트·RAG 설정·평가 결과 및 설계 근거 문서화

---

## Repository Philosophy

각 프로젝트는 독립된 저장소로 관리하며, 다음 원칙을 따릅니다.

- 구조화된 폴더 구성 (`accounts`, `products`, `chats`, `common`, `templates` 등)
- 데이터·문서·비밀값(`.env`) 분리 관리
- 설정·의존성·평가 항목 버전 관리
- 산출물 및 실험 기록 유지

---

## 📂 Main Repository

| 저장소 | 설명 |
|--------|------|
| [4th_project](https://github.com/SKN26-4th-1st/4th_project) | LG Home 웹 애플리케이션 및 LLM 파이프라인 |
