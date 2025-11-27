<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/water.css@2/out/water.css">

# 안녕하세요, 서정의 포트폴리오입니다.

## 🛠 Skills

* **Languages:** C#, Python
* **Engines & Tools:** Unity, Git
* **Core Competencies:**
    * **Unity Client Programming:** Player Logic, Map Editor
    * **Multiplayer Networking:** Custom Packet Optimization, Stress Test
    * **Systems Programming:** OS Architecture, Pintos Project
    * **Backend:** Flask, MongoDB, FastAPI


---

## 🚀 Key Projects

### 1. StackGuys (대규모 멀티플레이 레이스 게임)
**🔗 Repository:** [May-I-Game/stack-guys](https://github.com/May-I-Game/stack-guys)

'폴가이즈' 스타일의 실시간 멀티플레이어 레이스 게임입니다. 단일 세션 100명이 플레이 가능한 서버를 구축하고 <br>
이를 스케일 아웃하여 대규모 인원을 수용하는 아키텍처를 설계했습니다.

* **Role:** 서버 프로그래밍, 플레이어 로직, 맵 에디터, 부하 테스트 툴 개발
* **Tech Stack:** Unity, Unity Netcode for GameObjects(NGO), C#
* **Key Features:**
    * Headless Unity Server 기반 100명 단위 세션을 500개로 확장한 5만명 동시 접속이 가능한 서버 구조 설계 및 검증
    * 대규모 플레이어 동기화 문제해결을 위한 커스텀 패킷 배칭 및 최적화 구현
    * 생산성 향상을 위한 맵 에디터 구현 및 서버 부하 테스트를 위한 테스트 프로그램 자체 개발
 
## 🚀 시연영상 & 포스터

### 시연영상
> **[![Video Label](http://img.youtube.com/vi/dXCM9R4kjuk/0.jpg)](https://youtu.be/dXCM9R4kjuk)**

*(이미지를 클릭하면 시연 영상을 보실 수 있습니다)*

### 포스터
<details>
<summary><b>🖼 포스터 보기 (Click)</b></summary>
<br>
<img src="https://github.com/user-attachments/assets/db26e98f-4538-45ab-98a3-8562b34e27d5" width="600">
</details>

<br>
 
### 2. RustyDome_ (매트로배니아 플랫포머)
**🔗 Repository:** [Rostreaca/RustyDome_](https://github.com/Rostreaca/RustyDome_)

메트로배니아 스타일의 싱글플레이 플랫포머 게임입니다. 맵 탐험 요소와 캐릭터 성장 시스템을 중심으로 개발했습니다.

* **Role:** 시스템 설계 및 코어 구현
* **Tech Stack:** Unity, C#
* **Key Features:**
    * **정교한 캐릭터 조작:** 점프, 대시, 공격 등 플랫포머 특유의 조작감 및 물리 충돌 처리 구현.
    * **레벨 디자인 및 맵 시스템:** 탐험 가능한 맵 구조 설계 및 씬 전환 로직.
    * **게임 루프 및 상태 관리:** 플레이어 상태, 적 AI, 아이템 상호작용 등 핵심 게임 로직 구현.
 
<details>
<summary><b>🖼 인게임 스크린샷 보기 (Click)</b></summary>
<br>
<img width="590" height="399" alt="RustyDome_그림1" src="https://github.com/user-attachments/assets/96d0979c-7bbe-4c68-8cd2-5baded7f4e9e" />
<img width="599" height="400" alt="RustyDome_그림2" src="https://github.com/user-attachments/assets/514b4c00-b245-4ce7-ad7e-17c46d4bf14a" />
<img width="591" height="395" alt="RustyDome_그림3" src="https://github.com/user-attachments/assets/c25b6d7b-6692-4810-a6ca-b8faff41e071" />
</details>

<br>

### 3. JungleGame (웹 프로젝트)
**🔗 Repository:** [sjk2915/junglegame](https://github.com/sjk2915/junglegame)

GitHub 커밋 기반 경품에 응모하는 웹 서비스입니다. 백엔드 API와 DB 설계를 전담했습니다.

* **Role:** Back-End Developer & DB Architect
* **Tech Stack:** [Jinja2, TailwindCSS, Python (Flask), MongoDB]
* **Key Features:**
    * **백엔드 API 기능 구현**.
        * 페이지 렌더링(Login, Main 등)은 SSR 방식을 사용하여 SEO와 초기 로딩 속도를 고려.
        * 데이터 통신(잔디 그래프, 도전권 발급)은 JSON API로 비동기 처리하여 UX 향상.
    * **핵심 비즈니스 로직 구현**
        * **챌린지 시스템:** 커밋 기록 기반 1일 1회 도전권 발급 로직 (`/ticket`).
        * **응모 프로세스:** 응모권 기반 응모(`POST /lotto`) 및 당첨 결과 산출 알고리즘.
        * **시각화 데이터:** 깃 허브 사용자 활동(Grass) 데이터를 JSON으로 가공하여 프론트엔드에 제공.
    * **MongoDB(NoSQL) 스키마 설계**
        * `Users`: 사용자 인증 정보 및 `appList`(응모 내역), `attendanceList`(출석) 등 배열 필드를 활용한 활동 이력 관리.
        * `Product`: 경품의 가격 범위(`min/maxPrice`)와 응모 기간(`start/endDate`)을 관리하여 회차별 게임 운영 지원.
        * `Reward`: 회차별(`appRound`) 당첨자(`appUser`) 및 결과 히스토리 아카이빙.

---

## 📬 Contact
* **Email:** seo980620@gmail.com
* **GitHub:** [https://github.com/sjk2915](https://github.com/sjk2915)
* **Blog:** [https://seo980620.tistory.com/](https://seo980620.tistory.com)
