> Unity와 C#을 기반으로 한 게임 개발 역량과 OS, 네트워크 등 탄탄한 CS 기초를 갖추고 있습니다.
<br>

## 🛠 Skills

* **Languages:** C#, Python
* **Engines & Tools:** Unity, Git, docker
* **Unity Client & Tooling:**
   * FSM 기반의 확장성 있는 캐릭터 로직 설계 및 구현
   * 기획/아트 파트의 생산성을 높이는 Editor Scripting 및 커스텀 툴 개발
* **Multiplayer Networking:**
   * 대규모 동시 접속 처리를 위한 Headless Server 아키텍처 설계
   * 네트워크 대역폭 최적화를 위한 패킷 설계 및 동기화 로직 구현
* **Systems Programming (CS):**
   * OS 스케줄러/가상 메모리 구현을 통한 프로세스·스레드 구조 이해 (PintOS)
   * 멀티스레딩 환경에서의 동시성 제어 및 메모리 관리 역량
<br>

# 🚀 Key Projects

## 1. StackGuys (대규모 멀티플레이 레이스 게임)
**🔗 Repository:** [May-I-Game/stack-guys](https://github.com/May-I-Game/stack-guys)

'폴가이즈' 스타일의 실시간 멀티플레이어 레이스 게임입니다. 단일 세션 100명이 플레이 가능한 서버를 구축하고 
이를 스케일 아웃하여 대규모 인원을 수용하는 아키텍처를 설계했습니다.

* **Role:** 서버 프로그래밍, 플레이어 로직, 맵 에디터, 부하 테스트 툴 개발
* **Tech Stack:** Unity, Unity Netcode for GameObjects(NGO), C#
* **Key Features:**
    * **5만 CCU 서버 설계 및 검증:** Headless Unity Server 기반 최대 5만명 동시 접속이 가능한 서버 구조 설계 및 검증.
    * **서버 권위 캐릭터 조작:** 이동, 점프, 다이브, 잡기, 던지기 등 플레이어 액션을 서버에서 처리하는 권위 구조 구현.
    * **네트워크 동기화 패킷:** 대규모 플레이어 동기화 문제해결을 위한 커스텀 패킷 배칭 및 최적화 구현.
    * **맵 에디터, 부하 테스트 프로그램:** 생산성 향상을 위한 맵 에디터 구현 및 서버 부하 테스트를 위한 테스트 프로그램 자체 개발.
 
### 🎥 시연영상
**[![Video Label](http://img.youtube.com/vi/dXCM9R4kjuk/0.jpg)](https://youtu.be/dXCM9R4kjuk)**

*(이미지를 클릭하면 시연 영상을 보실 수 있습니다. 발표는 팀장이 진행하였습니다.)*

### 포스터
<details>
<summary><b>🖼 포스터 보기 (Click)</b></summary>
<br>
<img src="https://github.com/user-attachments/assets/db26e98f-4538-45ab-98a3-8562b34e27d5" width="600">
</details>

<br>
 
## 2. RustyDome_ (매트로배니아 플랫포머)
**🔗 Repository:** [Rostreaca/RustyDome_](https://github.com/Rostreaca/RustyDome_)

무기 조합과 캐릭터 커스터마이징이 가능한 메트로배니아 스타일의 싱글플레이 플랫포머 게임입니다.

* **Role:** 시스템 설계 및 코어 구현
* **Tech Stack:** Unity, C#
* **Key Features:**
    * **정교한 캐릭터 조작:** 점프, 대시, 공격콤보, 처형 등 캐릭터 조작 및 특수 공격 시스템 구현.
    * **게임 루프 및 상태 관리:** 플레이어 상태, 적 AI, 아이템 상호작용 등 핵심 게임 로직 구현.
    * **아이템 및 캐릭터 스탯 모듈:** `ScriptableObject`로 설계하여, 코드 수정 없이 기획 데이터(공격력, 옵션 등)를 유연하게 관리하고 확장성을 확보.
    * **UI 시스템 개발:** 맵, 인벤토리, 커스터마이징, 옵션 등 UI 시스템 설계 및 개발.
    * **레벨 디자인 및 맵 시스템:** 메트로배니아 특유의 비선형 맵 구조 설계 및 씬 전환 로직.
 
<details>
<summary><b>🖼 인게임 스크린샷 보기 (Click)</b></summary>
<br>
<img width="600" height="400" alt="RustyDome_그림1" src="https://github.com/user-attachments/assets/96d0979c-7bbe-4c68-8cd2-5baded7f4e9e" />
<img width="600" height="400" alt="RustyDome_그림2" src="https://github.com/user-attachments/assets/514b4c00-b245-4ce7-ad7e-17c46d4bf14a" />
<img width="600" height="400" alt="RustyDome_그림3" src="https://github.com/user-attachments/assets/c25b6d7b-6692-4810-a6ca-b8faff41e071" />
</details>

<br>

### 🚀 주요 설계 및 구현 (Architectural Deep Dive)

이 프로젝트는 데이터와 로직을 명확하게 분리하는 **데이터 주도 설계(Data-Driven Design)** 를 핵심 아키텍처로 채택했습니다.
특히 **ScriptableObject(SO)** 를 적극적으로 활용하여 기획 데이터와 게임 로직 간의 의존성을 최소화하고, 코드 수정 없이도 콘텐츠를 확장할 수 있는 유연한 구조를 구현했습니다.

#### 1. ScriptableObject 기반의 계층적 아이템 및 무기 시스템

게임의 핵심 요소인 무기와 아이템은 SO를 통해 계층적으로 설계되었습니다. 
이는 단순한 데이터 컨테이너를 넘어, 객체 지향의 상속 구조를 활용하여 시스템의 확장성과 재사용성을 극대화할 수 있도록 설계되었습니다..

- **`Item` (Base SO):** 모든 아이템이 공통으로 가지는 속성(아이콘, 이름, 설명 등)을 정의하는 최상위 ScriptableObject입니다.
- **`Weapon` (Abstract Class):** `Item`을 상속받아 무기류 아이템의 기본 데이터(대미지, 파워 소모량)와 기능(`Use()` 추상 메서드)을 정의합니다. 이를 통해 '모든 무기는 아이템'이라는 명확한 "is-a" 관계를 형성합니다.
- **`MeleeWeapon` / `RangeWeapon` / `SpecialWeapon` (Concrete Classes):** `Weapon`을 상속받아 근접, 원거리 등 무기 타입별로 특화된 데이터(스턴 대미지, 스킬 쿨타임 등)와 기본 로직을 구현합니다.
- **`Crowbar`, `ScrapGun` 등 (Concrete SO Assets):** 최종적으로 `MeleeWeapon` 같은 클래스를 상속받는 구체적인 무기 SO를 정의합니다. (`[CreateAssetMenu]`) 게임 디자이너는 이 에셋 파일을 통해 코드 한 줄 없이 '쇠지렛대', '고철총' 등 새로운 무기를 생성하고, 인스펙터 창에서 모든 스탯을 직관적으로 수정할 수 있습니다.

```csharp
// 1. 기본 아이템 데이터 (SO)
// Assets/Scripts/UI/Item.cs
[CreateAssetMenu(fileName = "Item", menuName = "ScriptableObjects/Item", order = 1)]
public class Item : ScriptableObject
{
    public string itemName;
    public Sprite icon;
    // ...
}

// 2. 무기 타입으로 확장 (상속)
// Assets/Scripts/Weapon/Weapon.cs
public abstract class Weapon : Item
{
    public int dmg;
    public abstract void Use();
    // ...
}

// 3. 근접 무기로 구체화
// Assets/Scripts/Weapon/MeleeWeapon.cs
public class MeleeWeapon : Weapon
{
    public int stunDmg;
    public override void Use() { /* 근접 공격 로직 */ }
    // ...
}

// 4. 최종 무기 에셋 생성
// Assets/Scripts/Weapon/MeleeWeapon/Crowbar.cs
[CreateAssetMenu(fileName = "Crowbar", menuName = "ScriptableObjects/MeleeWeapon/Crowbar")]
public class Crowbar : MeleeWeapon
{
    // 에셋 메뉴에서 생성하면 이 클래스 타입의 SO가 만들어집니다.
    // 모든 데이터는 부모 클래스에 정의되어 있으며, 인스펙터에서 설정됩니다.
}
```

#### 2. 데이터와 로직의 명확한 분리

`PlayerCombat`과 같은 `MonoBehaviour` 스크립트는 이러한 무기 SO를 참조하여 실제 전투 로직을 수행합니다.

- `PlayerCombat`은 현재 장착된 무기 SO(`player.meleeWeapon`)에 접근하여 공격력, 애니메이션 이름, 파워 소모량 등의 데이터를 가져와 사용합니다.
- 덕분에 무기의 밸런스를 조정하거나 공격 애니메이션을 변경할 때 `PlayerCombat` 코드를 전혀 수정할 필요가 없습니다. 오직 해당 무기의 SO 에셋 파일 값만 변경하면 모든 로직에 즉시 반영됩니다.
- 이는 유지보수 비용을 크게 절감하고, 기획자와 프로그래머 간의 협업 효율을 극대화합니다.

```csharp
// PlayerCombat.cs - SO 데이터를 소비하는 로직
public class PlayerCombat : MonoBehaviour
{
    private PlayerController player; // 플레이어 정보

    public void MeleeAttack(EnemyController enemy)
    {
        // meleeWeapon은 ScriptableObject 에셋입니다.
        // SO에 정의된 데이터(stunDmg)를 가져와 로직에 사용합니다.
        enemy.GetDamage(player.meleeDmg, player.meleeWeapon.stunDmg);
    }

    public void OnMeleeAttackBegin()
    {
        // SO의 데이터를 참조하여 파워를 소모합니다.
        player.powerNow -= player.meleeWeapon.powerCon;
        
        // SO의 데이터로 애니메이션을 제어합니다.
        animator.SetBool(player.meleeWeapon.animName, true);
    }
}
```
이처럼 `RustyDome_`은 확장성과 유지보수성을 최우선으로 고려한 설계를 통해, 복잡한 게임 시스템을 효율적으로 구축한 경험을 보여주는 프로젝트입니다.

<br>

## 3. JungleGame (Github 연동 추첨 웹 서비스)
**🔗 Repository:** [sjk2915/junglegame](https://github.com/sjk2915/junglegame)

GitHub 커밋 기반 경품에 응모하는 웹 서비스입니다. 백엔드 API와 DB 설계를 전담했습니다.

* **Role:** Back-End Developer & DB Architect
* **Tech Stack:** Jinja2, TailwindCSS, Python (Flask), MongoDB
* **Key Features:**
     * **SSR Rendering**: 페이지 렌더링(Login, Main 등)은 SSR 방식을 사용하여 SEO와 초기 로딩 속도를 고려.
     * **비즈니스 로직 구현:** 응모권 기반 응모(`POST /lotto`) 및 당첨 결과 산출 알고리즘.
     * **데이터 시각화:** GitHub 커밋 활동을 JSON으로 가공하여 잔디 그래프로 시각화.
     * **MongoDB 스키마 설계:** 복잡한 Join 없이 단일 쿼리로 DB를 조회하도록 읽기 성능 최적화.

---

## 📬 Contact
* **Email:** [seo980620@gmail.com](mailto:seo980620@gmail.com)
* **GitHub:** [https://github.com/sjk2915](https://github.com/sjk2915)
* **Blog:** [https://seo980620.tistory.com/](https://seo980620.tistory.com)

<style>
  header, .site-header, #header {
    display: none !important;
  }
  body, .main-content {
    margin-top: 50px !important;
  }
</style>
