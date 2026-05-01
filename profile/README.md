# SKN26 4th 1st Team - None

팀의 메인 산출물은 **PICKLE** (신대방삼거리 맛집 추천 챗봇)입니다. 다이닝코드에서 수집한 **식당 100곳·메뉴 2,000여 개·리뷰 400여 건**을 **SQLite + 텍스트 임베딩(base64 저장)** 으로 구축하고, **LangGraph**로 *라우팅(조건 탐색 vs 엔티티 직접 검색) → JSON Schema 슬롯 추출 → DB·코사인 유사도 검색 → 근거 기반 답변* 파이프라인을 이어 **Streamlit** UI와 **Kakao Map** 연동까지 한 흐름으로 묶었습니다. “DB에 없는 식당을 지어내지 않는다”는 **Grounded 추천**과 리뷰·태그·메뉴를 견고히 잇는 **데이터 모델**을 앞에 두는 구조가 특징입니다.

평가 측면에서는 `src_test` / `src_test2` / `src_test3`에 **골드셋(고정·임베딩 유형, 총 50케이스)** 생성, `run_qa` 기반 자동 점수화, **HTML·노트북 대시보드**로 회귀를 볼 수 있게 해 두어, 데모를 넘어 **재현 가능한 품질 관리**를 지향합니다.

> 상세 아키텍처·DB 스키마·실행 방법은 조직 저장소의 [4th_project/README.md](https://github.com/SKN26-3rd-3rd/3rd_project/blob/main/README.md)를 참고하세요.

---

## 👥 Team
<table>
  <tr>
    <td align="center">
      <img src="https://github.com/gieun-Park.png" width="110px;" /><br />
      <b>박기은</b><br />
      <a href="https://github.com/gieun-Park">@gieun-Park</a>
    </td>
    <td align="center">
      <img src="https://github.com/minhyeok328.png" width="110px;" /><br />
      <b>서민혁</b><br />
      <a href="https://github.com/minhyeok328">@minhyeok328</a>
    </td>
    <td align="center">
      <img src="https://github.com/Ocean-2930.png" width="110px;" /><br />
      <b>유동현</b><br />
      <a href="https://github.com/Ocean-2930">@Ocean-2930</a>
    </td>
    <td align="center">
      <img src="https://github.com/dimolto3.png" width="110px;" /><br />
      <b>윤정연</b><br />
      <a href="https://github.com/dimolto3">@dimolto3</a>
    </td>
    <td align="center">
      <img src="https://github.com/leere2424.png" width="110px;" /><br />
      <b>이레</b><br />
      <a href="https://github.com/leere2424">@leere2424</a>
    </td>
    <td align="center">
      <img src="https://github.com/wjdduddlf112.png" width="110px;" /><br />
      <b>정영일</b><br />
      <a href="https://github.com/wjdduddlf112">@wjdduddlf112</a>
    </td>
  </tr>
</table>

---

## 🛠 Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-121212?style=for-the-badge&logo=chainlink&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)

![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![Beautiful Soup](https://img.shields.io/badge/BeautifulSoup-4B8BBE?style=for-the-badge)
![Selenium](https://img.shields.io/badge/Selenium-43B02A?style=for-the-badge&logo=selenium&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![.env](https://img.shields.io/badge/python--dotenv-000000?style=for-the-badge)
![Kakao Map](https://img.shields.io/badge/Kakao_Maps-FFCD00?style=for-the-badge)

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
[![Notion](https://img.shields.io/badge/Notion-Project_Page-000000?style=for-the-badge&logo=notion&logoColor=white)](https://efficacious-sweater-208.notion.site/PICKLE-33b229ee8c45804f9debf203db276faf?source=copy_link)


---

## Team Identity

우리는 단순히 LLM 데모를 만드는 팀이 아니라  
요구사항 정의 → **크롤링·정제·DB·임베딩** 등 데이터 파이프라인 → **RAG·LangGraph·에이전트** 설계 → 프롬프트·도구·체인 구성 →  
**골드셋·지표 기반 평가**와 가드레일 → Streamlit·지도 연동 등 **서비스 UX**까지  
한 프로젝트 안에서 끊기지 않게 잇는 엔지니어링 중심 팀입니다.

---

## Core Capabilities

- **하이퍼로컬 도메인 RAG**: 좁은 지역·풍부한 메타(카테고리·태그·메뉴·리뷰)를 전제로 한 **Grounded** 추천·QA 설계
- **라우터·슬롯·검색·생성** 분리: 질의 유형 분기(예: `embedding` / `fixed`), JSON Schema 강제 슬롯, **SQLite + 코사인 유사도** 후보 수집, 시스템 프롬프트로 답변 생성
- LangChain·**LangGraph** 기반 체인·에이전트·도구 연동 및 OpenAI(채팅·임베딩) API 활용
- 프롬프트·시스템 지침 설계와 응답 품질·할루시네이션 완화
- **DB 기반 골드셋**·가중 점수·JSON/HTML 리포트로 `run_qa` 회귀 점검(프로젝트 내 `src_test*`)
- 재현 가능한 설정·버전 관리(프롬프트, 체인, 의존성, DB 스냅샷)
- Git 기반 협업 (PR / Issue / Conventional Commits)
- **Streamlit + Kakao Map** 프로토타입·서비스 UI 구성

---

## Working Method

- Issue 기반 작업 분리
- Branch 전략 준수
- Conventional Commit 사용
- PR 리뷰 후 Merge
- 프롬프트·RAG 설정·평가 결과 및 설계 근거 문서화

---

## Repository Philosophy

각 프로젝트는 독립된 저장소로 관리하며  
다음 원칙을 따릅니다:

- 구조화된 폴더 구성 (`src` 파이프라인, `database` 수집·전처리·SQL, `frontend` UI 등)
- 데이터·문서·비밀값(`.env`) 분리 관리
- 프롬프트·체인·모델 설정·**평가 스크립트** 버전 관리
- 산출물·실험 로그·골드셋·**평가 리포트** 기록 유지

---