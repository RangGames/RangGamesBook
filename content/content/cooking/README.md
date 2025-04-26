# 🫕 요리 (Cooking)

서버 고유의 다양한 요리를 만들어 특별한 효과를 얻거나 판매할 수 있습니다. 요리는 전용 UI와 장비를 통해 진행됩니다.

### **요리 방법 (How to Cook - Step-by-Step)**

요리를 만들기 위한 전체 과정은 다음과 같습니다:

1.  **레시피 확인 (Check Recipe):**
    *   먼저 만들고 싶은 요리의 레시피(필요 재료, 조리법 등)를 확인합니다.
    *   명령어: `/레시피`

2.  **레시피 구매 (Purchase Recipe):**
    *   원하는 요리의 레시피를 아직 배우지 않았다면, `요리 상점 (Cooking Shop)` 등 지정된 장소에서 구매해야 합니다. (레시피는 일반적으로 한 번 구매하면 영구적으로 사용 가능합니다.)

3.  **재료 준비 및 보관 (Prepare & Store Ingredients):**
    *   레시피에 필요한 재료들을 모읍니다. (채집, 농사, 낚시, 사냥, 구매 등)
    *   준비된 재료는 요리 시스템이 인식할 수 있도록 전용 보관 공간에 넣어야 합니다.
    *   명령어: `/요리 재료` 또는 `/요리 가마솥` (서버 설정에 따라 둘 중 하나 또는 둘 다 사용될 수 있으며, 재료를 넣는 UI가 열립니다.)

4.  **요리 시작 (Start Cooking):**
    *   재료가 준비되면 요리 제작 UI를 엽니다.
    *   명령어: `/요리`
    *   UI 내에서 만들고자 하는 요리(습득한 레시피 목록)를 선택한 후, '제작하기' 버튼을 클릭합니다.

    <div align="left"><figure><img src="../../../.gitbook/assets/cook.png" alt="요리 제작 UI"><figcaption><p>'/요리' 명령어 실행 시 나타나는 UI</p></figcaption></figure></div>

5.  **제작 확인 (Confirm Production):**
    *   제작을 시작하면 채팅창에 확인을 위한 안내가 나타날 수 있습니다. (서버 구현 방식에 따라 다름)
    *   안내에 따라 만들려는 **요리에 해당하는 숫자**를 채팅창에 입력하여 최종적으로 제작을 확정합니다.

6.  **요리 완료 및 수령 (Finish & Retrieve):**
    *   요리가 완성되면 알림이 표시됩니다.
    *   완성된 요리는 요리 전용 가방에서 꺼내 인벤토리로 옮겨야 합니다.
    *   명령어: `/요리 가방`

---

### **요리 장비: 요리사의 비법 (Cooking Equipment: Cook's Secret Recipe Book)**

요리 효율과 결과물에 영향을 미치는 핵심 장비입니다.

*   **획득 방법:** `요리 상점 NPC 하루토`를 우클릭하여 기본 `요리사의 비법`을 얻을 수 있습니다.
*   **기본 기능:** 요리 레시피를 저장하고 요리 관련 능력치를 제공합니다.
*   **기본 슬롯:** 처음 획득 시 **2줄(칸)**의 재료 또는 보조 아이템 슬롯을 가집니다.

    <div align="left"><figure><img src="../../../.gitbook/assets/제목 없음-9 (1).png" alt="요리사의 비법 아이템"><figcaption><p>요리사의 비법 (Cook's Secret Recipe Book)</p></figcaption></figure></div>
    <div align="left"><figure><img src="../../../.gitbook/assets/2줄.png" alt="기본 슬롯 2칸 상태"><figcaption><p>기본 슬롯 2칸</p></figcaption></figure></div>

*   **슬롯 확장 (Slot Expansion):**
    *   `잠금 해제 열쇠` 아이템을 사용하여 `요리사의 비법` 슬롯을 확장할 수 있습니다.
    *   **일반 잠금 해제 열쇠:** 사용 시 **30% 확률**로 슬롯 한 줄 확장 성공.
    *   **고급 잠금 해제 열쇠:** 사용 시 **100% 확률**로 슬롯 한 줄 확장 성공.

    <div align="left"><figure><img src="../../../.gitbook/assets/잠금해제열쇠 (1).png" alt="일반 잠금 해제 열쇠"><figcaption><p>잠금 해제 열쇠 (Unlock Key)</p></figcaption></figure> <figure><img src="../../../.gitbook/assets/고급해제열쇠 (1).png" alt="고급 잠금 해제 열쇠"><figcaption><p>고급 잠금 해제 열쇠 (Advanced Unlock Key)</p></figcaption></figure></div>
    <div align="left"><figure><img src="../../../.gitbook/assets/3줄.png" alt="확장된 슬롯 상태"><figcaption><p>열쇠로 슬롯 확장된 모습</p></figcaption></figure></div>

---

### **요리사의 비법 강화 (Upgrading the Secret Recipe Book)**

`요리사의 비법`에 추가적인 능력치를 부여하거나 효과를 강화할 수 있습니다.

*   **강화 아이템:** `미스테리 큐브 (Mystery Cube)`, `어센틱 큐브 (Authentic Cube)` 등을 사용합니다. (큐브 종류에 따라 효과나 성공률이 다를 수 있습니다.)
*   **강화 방법:**
    1.  강화에 사용할 **큐브 아이템**을 손에 듭니다.
    2.  큐브를 들고 **우클릭**하면 강화 전용 UI가 열립니다.
    *   명령어 입력 대신, 큐브 우클릭 액션으로 UI를 여는 방식입니다.
    *   UI가 열리면 강화할 `요리사의 비법`을 넣고 강화를 진행합니다. (UI 내에서 강화 확률, 비용, 결과 등을 확인할 수 있습니다.)

    <div align="left"><figure><img src="../../../.gitbook/assets/ㄴㄴ.png" alt="요리 장비 강화 UI"><figcaption><p>큐브 우클릭 시 나타나는 '/요리 장비' 강화 UI</p></figcaption></figure></div>