<!--
GitHub 프로필 README · tyfmq123-hub
공개 저장소 tyfmq123-hub/tyfmq123-hub의 루트에 이 README.md를 배치하고,
assets/profile-banner.svg도 같은 상대 경로로 업로드하세요.
적용 안내: https://docs.github.com/en/account-and-profile/how-tos/profile-customization/managing-your-profile-readme
공개 저장소의 기본 브랜치와 커밋 기록을 2026-10-06 기준으로 확인했습니다.
TODO: 공개할 실명, 이메일, 포트폴리오 링크를 추가하세요.
TODO: 프로젝트별 실제 개발 기간과 진행 상태를 확인하세요.
-->

<p align="center">
  <img src="./assets/profile-banner.svg" alt="tyfmq123-hub — 플레이를 코드로 만듭니다. Unity와 C#으로 전투와 상호작용을 구현합니다." width="100%">
</p>

<p align="center">
  <strong>게임 플레이 · UI · XR 인터랙션 · 일정 자동화</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Unity-182635?style=flat-square&amp;logo=unity&amp;logoColor=white" alt="Unity">
  <img src="https://img.shields.io/badge/C%23-285547?style=flat-square" alt="C#">
  <img src="https://img.shields.io/badge/Python-243c54?style=flat-square&amp;logo=python&amp;logoColor=FFD166" alt="Python">
  <img src="https://img.shields.io/badge/SQLite-243c54?style=flat-square&amp;logo=sqlite&amp;logoColor=white" alt="SQLite">
  <img src="https://img.shields.io/badge/Discord-444d88?style=flat-square&amp;logo=discord&amp;logoColor=white" alt="Discord">
  <img src="https://img.shields.io/badge/Git-593b32?style=flat-square&amp;logo=git&amp;logoColor=white" alt="Git">
</p>

<p align="center">
  <a href="#소개">소개</a> ·
  <a href="#대표-프로젝트와-주요-기능">대표 프로젝트</a> ·
  <a href="#기술-스택">기술 스택</a> ·
  <a href="#개발-기록">개발 기록</a>
</p>


## 소개

안녕하세요, **tyfmq123-hub**입니다.

Unity와 C#을 중심으로 게임의 전투 로직과 UI를 구현하고, XR 장비 상호작용과 Python 일정 자동화로 작업 범위를 넓히고 있습니다. 슈팅 게임 학습 프로젝트부터 3인 팀 디펜스 게임, 보호구 준비실 데모, Discord 봇까지 코드와 개발 기록을 이곳에 모았습니다.

대표 작업인 **Ratchemy Defense**에서는 아군 유닛과 스킬, 소환 카드, 스토리·결과 UI, 밸런스 시뮬레이터를 구현하고 팀의 Pull Request를 통합했습니다.


## 개발자

| 항목 | 내용 |
| --- | --- |
| GitHub | [@tyfmq123-hub](https://github.com/tyfmq123-hub) |
| 주요 작업 | Unity 게임 플레이·UI 구현, XR 상호작용, Python 봇 개발 |
| 협업 경험 | Ratchemy Defense 3인 팀 프로젝트의 아군·결과 UI 작업 및 PR 통합 |

<!-- TODO: 실명과 공개 가능한 연락처·포트폴리오를 추가하세요. -->


## 대표 프로젝트와 주요 기능

### 01 · [Ratchemy Defense](https://github.com/tyfmq123-hub/Ratchemy-Defense)

**유닛을 소환하고 배터리의 열폭주를 막는 2D 레인 디펜스 팀 프로젝트**

서로 다른 역할의 아군을 조합해 적 웨이브와 보스를 상대합니다. 3인 팀으로 전투, 기지·웨이브 관리, 씬 흐름과 UI를 나누어 구현했습니다.

- **아군 전투와 소환:** 5종 아군의 공격·스킬을 공통 기반 클래스 위에 구현했습니다. 카드 데이터와 코스트를 연결해 소환하고, 사망 시 코스트 일부를 환급합니다.
- **스토리와 결과 UI:** 만화 컷의 앞뒤 이동·자동 넘김과 승리·패배 결과 화면을 구현했습니다. HP·스킬 쿨다운 표시와 사운드도 전투 흐름에 연결했습니다.
- **밸런스 점검 도구:** 프리팹·ScriptableObject의 스탯으로 반복 전투를 시뮬레이션하고 리포트를 생성합니다. 브라우저 도구에서는 조합과 임시 스탯을 바꾸어 추정 승률을 비교할 수 있습니다.

`Unity` `C#` `URP 2D` `ScriptableObject` `uGUI` `JSON`

[아군 구현](https://github.com/tyfmq123-hub/Ratchemy-Defense/tree/develop/Assets/_Workspaces/Member_Jeon/1.Scripts/PlayerUnit) · [웹 밸런스 도구](https://github.com/tyfmq123-hub/Ratchemy-Defense/tree/develop/Assets/_Workspaces/Member_Jeon/BalanceSimWeb) · [QA 문서](https://github.com/tyfmq123-hub/Ratchemy-Defense/blob/develop/Docs/QA_Ratchemy_Defense.md)

### 02 · [HCl PPE 준비실](https://github.com/tyfmq123-hub/HCl-PPE-Room-Build)

**보호구 착용과 대응 장비 준비를 단계별로 연습하는 Unity XR 데모**

보호구를 올바른 순서로 착용하고 필요한 장비를 준비하는 상호작용을 구현한 프로젝트입니다. 저장소에는 준비실 소스와 Windows 64비트 실행 데모가 함께 정리되어 있습니다.

- **순서와 준비 상태 관리:** 보호구 착용 순서를 관리하고 대응 가방·폐기 용기의 준비 상태를 별도로 검증합니다. 체크리스트로 진행 상황을 표시합니다.
- **장비 상호작용과 안내:** 손·레이 기반 장비 잡기와 착용 판정을 지원합니다. 단계와 오류에 따라 음성 안내와 한국어 자막을 표시합니다.

`Unity` `C#` `XR Interaction Toolkit` `OpenXR` `XR Hands`

[착용 순서 코드](https://github.com/tyfmq123-hub/HCl-PPE-Room-Build/blob/main/Assets/1.JSR/Scripts/PPESequenceManager.cs) · [실행 안내](https://github.com/tyfmq123-hub/HCl-PPE-Room-Build/blob/main/README.md)

### 03 · [Discord 대회 일정 봇](https://github.com/tyfmq123-hub/Discoad-Bot)

**대회 일정 검색부터 개인 일정 저장·알림까지 연결하는 Python 봇**

공개 Google Sheets의 카드게임 대회 정보를 가져와 Discord에서 검색하고 저장합니다. 여러 곳에 흩어진 일정 확인과 시작 전 알림을 한 흐름으로 묶었습니다.

- **일정 수집과 검색:** 이벤트 페이지의 Google Sheets 링크를 찾아 CSV를 가져오고, 한국어 날짜·시간을 해석해 SQLite에 저장합니다. 매장·날짜·회차로 대회를 검색할 수 있습니다.
- **개인 일정과 알림:** 대회 일정과 직접 등록한 일정을 관리하고, 저장된 알림 시각을 확인해 Discord DM을 보냅니다.

`Python` `discord.py` `aiohttp` `SQLite` `Google Sheets CSV`

[대회 명령](https://github.com/tyfmq123-hub/Discoad-Bot/blob/main/commands/tournament.py) · [일정 관리](https://github.com/tyfmq123-hub/Discoad-Bot/blob/main/commands/schedule.py) · [알림 처리](https://github.com/tyfmq123-hub/Discoad-Bot/blob/main/reminders.py)


## 학습과 협업 프로젝트

| 프로젝트 | 주요 구현 |
| --- | --- |
| [2d-vertical-shooter](https://github.com/tyfmq123-hub/2d-vertical-shooter) | JSON·코루틴 기반 적 생성, 파워업·폭탄·리스폰, 스크롤 배경 타일 재활용 |
| [puri-2d-Speceshooter](https://github.com/tyfmq123-hub/puri-2d-Speceshooter) | 11개 JSON 웨이브, 적·탄환·아이템 오브젝트 풀 통합과 확장, 점수·목숨 UI |
| [mouse-SpaceShooter](https://github.com/tyfmq123-hub/mouse-SpaceShooter) | 마우스 클릭 발사, 추종 기체, 네 가지 보스 탄막, 오브젝트 풀링 |

`2d-vertical-shooter`와 `mouse-SpaceShooter`는 저장소에 명시된 골드메탈 2D 슈팅 학습 콘텐츠를 바탕으로 구현한 프로젝트입니다.


## 기술 스택

공개 프로젝트에서 사용한 기술을 분야별로 정리했습니다.

| 분야 | 기술 | 활용 |
| --- | --- | --- |
| 언어 | C#, Python | 게임 로직·UI, Discord 봇 |
| 게임 엔진 | Unity 6 | 2D 슈팅·디펜스, PPE 준비실 |
| 그래픽·UI | URP, uGUI, TextMesh Pro | 화면 렌더링, 카드·체력·결과 UI |
| XR | XR Interaction Toolkit, OpenXR, XR Hands | 손·레이 상호작용과 장비 착용 |
| 데이터 | ScriptableObject, JSON, SQLite | 유닛 스탯, 웨이브, 일정 저장 |
| 외부 연동 | Discord API, Google Sheets CSV | 명령·DM 알림, 대회 일정 수집 |
| 협업 | Git, GitHub, Git LFS | 기능 브랜치·PR 통합, 대형 자산 관리 |


## 개발 기록

공개 기본 브랜치의 **커밋 기록 기준**이며, 날짜는 한국 시간입니다. 실제 개발 시작·종료일은 별도 확인이 필요합니다.

| 기록 범위 | 프로젝트 | 확인된 작업 |
| --- | --- | --- |
| 2026.04.23 ~ 2026.04.28 | 2d-vertical-shooter | 세로 스크롤 슈팅과 데이터 기반 적 생성 |
| 2026.04.28 ~ 2026.05.01 | puri-2d-Speceshooter | 팀 작업, JSON 웨이브 연동, 풀 매니저 통합 |
| 2026.05.04 ~ 2026.05.06 | mouse-SpaceShooter | 클릭 발사, 추종 기체, 보스 탄막 |
| 2026.05.22 ~ 2026.06.16 | Ratchemy Defense | 아군·카드·결과 UI, 밸런스 도구, 제출용 브랜치 통합 |
| 2026.06.18 | Discoad-Bot | 일정 봇 소스 공개 스냅샷 |
| 2026.09.18 | HCl-PPE-Room-Build | PPE 준비실 소스 공개 스냅샷 |

<!-- TODO: 실제 개발 기간, 주요 이정표와 현재 진행 상태를 확인해 갱신하세요. -->


## 개발 환경

| 항목 | 확인된 설정·문서 |
| --- | --- |
| Unity 에디터 | 슈팅 3개 프로젝트: **6000.4.1f1** / Ratchemy Defense·PPE 준비실: **6000.4.8f1** |
| Unity 패키지 | URP **17.4.0**, Input System **1.19.0**, uGUI **2.0.0** |
| XR 패키지 | XR Interaction Toolkit **3.4.1**, OpenXR **1.16.1**, XR Hands **1.7.3** — PPE 준비실 기준 |
| 봇 의존성 | `discord.py>=2.3.0`, `aiohttp>=3.9.0`, `python-dotenv>=1.0.0`, `tzdata>=2023.3` — 설치 하한 |
| IDE·작업 도구 | Ratchemy Defense 팀 문서에 **Cursor·Unity·GitHub** 명시 |
| 빌드 대상 | Ratchemy Defense·PPE 준비실의 **Windows 64비트** 실행 빌드 |

<!-- TODO: 실제 개발 OS, 프로젝트별 사용 IDE와 Python 런타임 버전을 추가하세요. -->

버전은 각 저장소의 `ProjectVersion.txt`, `manifest.json`, `packages-lock.json`, `requirements.txt`와 프로젝트 문서를 기준으로 정리했습니다.


## 연락

[GitHub 프로필](https://github.com/tyfmq123-hub) · [전체 저장소](https://github.com/tyfmq123-hub?tab=repositories)

<!-- TODO: 공개할 이메일과 포트폴리오 URL을 추가하세요. -->
