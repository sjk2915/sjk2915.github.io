# 안녕하세요, 서정의 포트폴리오입니다.

## 🛠 Skills

* **Languages:** C#, Python
* **Engines & Tools:** Unity, Git
* **Core Competencies:**
    * **Unity Client Programming:** Player Logic, Map Editor
    * **Multiplayer Networking:** Custom Packet Optimization, Stress Test
    * **Systems Programming:** OS Architecture, Pintos Project
    * **Web Development:** Flask, MongoDB, FastAPI

---

## 🚀 Key Projects

### 1. StackGuys (대규모 멀티플레이 레이스 게임)
**🔗 Repository:** [May-I-Game/stack-guys](https://github.com/May-I-Game/stack-guys)

'폴가이즈' 스타일의 실시간 멀티플레이어 레이스 게임입니다. 단일 세션 100명이 플레이 가능한 서버를 구축하고 
이를 스케일 아웃하여 대규모 인원을 수용하는 아키텍처를 설계했습니다.

* **Role:** 서버 프로그래밍, 플레이어 로직, 맵 에디터, 부하 테스트 툴 개발
* **Tech Stack:** Unity, Unity Netcode for GameObjects(NGO), C#
* **Key Features:**
    * **5만명 접속 검증된 서버:** Headless Unity Server 기반 최대 5만명 동시 접속이 가능한 서버 구조 설계 및 검증.
    * **서버 권위 캐릭터 조작:** 이동, 점프, 다이브, 잡기, 던지기 등 플레이어 액션을 서버에서 처리하는 권위 구조 구현.
    * **네트워크 동기화 패킷:** 대규모 플레이어 동기화 문제해결을 위한 커스텀 패킷 배칭 및 최적화 구현.
    * **맵 에디터, 부하 테스트 프로그램:** 생산성 향상을 위한 맵 에디터 구현 및 서버 부하 테스트를 위한 테스트 프로그램 자체 개발.
 
## 시연영상 & 포스터

### 🎥 시연영상
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

무기 조합과 캐릭터 커스터마이징이 가능한 메트로배니아 스타일의 싱글플레이 플랫포머 게임입니다.

* **Role:** 시스템 설계 및 코어 구현
* **Tech Stack:** Unity, C#
* **Key Features:**
    * **정교한 캐릭터 조작:** 점프, 대시, 공격콤보 등 플랫포머 특유의 조작감 및 물리 충돌 처리 구현.
    * **게임 루프 및 상태 관리:** 플레이어 상태, 적 AI, 아이템 상호작용 등 핵심 게임 로직 구현.
    * **아이템 및 캐릭터 스탯 모듈:** `ScriptableObject`로 설계하여, 코드 수정 없이 기획 데이터(공격력, 옵션 등)를 유연하게 관리하고 확장성을 확보.
    * **UI 시스템 개발:** 맵, 인벤토리, 커스터마이징, 옵션 등 UI 시스템 설계 및 개발
    * **레벨 디자인 및 맵 시스템:** 메트로배니아 특유의 비선형 맵 구조 설계 및 씬 전환 로직.
 
<details>
<summary><b>🖼 인게임 스크린샷 보기 (Click)</b></summary>
<br>
<img width="600" height="400" alt="RustyDome_그림1" src="https://github.com/user-attachments/assets/96d0979c-7bbe-4c68-8cd2-5baded7f4e9e" />
<img width="600" height="400" alt="RustyDome_그림2" src="https://github.com/user-attachments/assets/514b4c00-b245-4ce7-ad7e-17c46d4bf14a" />
<img width="600" height="400" alt="RustyDome_그림3" src="https://github.com/user-attachments/assets/c25b6d7b-6692-4810-a6ca-b8faff41e071" />
</details>

<br>

### 3. JungleGame (Github 연동 추첨 웹 서비스)
**🔗 Repository:** [sjk2915/junglegame](https://github.com/sjk2915/junglegame)

GitHub 커밋 기반 경품에 응모하는 웹 서비스입니다. 백엔드 API와 DB 설계를 전담했습니다.

* **Role:** Back-End Developer & DB Architect
* **Tech Stack:** Jinja2, TailwindCSS, Python (Flask), MongoDB
* **Key Features:**
     * **SSR Rendering**: 페이지 렌더링(Login, Main 등)은 SSR 방식을 사용하여 SEO와 초기 로딩 속도를 고려.
     * **비즈니스 로직 구현:** 응모권 기반 응모(`POST /lotto`) 및 당첨 결과 산출 알고리즘.
     * **데이터 시각:** GitHub 커밋 활동을 JSON으로 가공하여 잔디 그래프로 시각화.
     * **MongoDB 스키마 설계:** 복잡한 Join 없이 단일 쿼리로 사용자 활동을 조회하도록 읽기 성능 최적화.

---

## 📬 Contact
* **Email:** [seo980620@gmail.com](mailto:seo980620@gmail.com)
* **GitHub:** [https://github.com/sjk2915](https://github.com/sjk2915)
* **Blog:** [https://seo980620.tistory.com/](https://seo980620.tistory.com)
