---
description: PSM Editor와 Toolbar에 대해 설명한다.
---

# PSM Editor

### 3.3. PSM Editor <a href="#d5e2894" id="d5e2894"></a>

메인 화면에서 **\[File] > \[New Editor] > \[PSM Editor]** 메뉴를 선택하거나 Tab 영역의 \[+버튼]  > \[PSM Editor]를  클릭하면 **PSM Editor 화면**에서 SQL 문장 뿐만을  아니라 PSM(Persistent Stored Module)문장을 작성하고 실행할 수 있다.

PSM Editor는 PSM 문장을 입력하고 실행할 수 있는 화면 상단의 **Editor 영역**과 PSM 문장의 실행 결과나 실행 계획을 볼 수 있는 화면 하단의 **Result View 영역**으로 구성된다. 또한 PSM Editor 화면 왼쪽에는 **Tree 영역**으로 구성된다. Tree 영역에 ![](https://technet.tmax.co.kr/upload/download/online/tibero/pver-20170425-000001/user-guide/resources/figure\_refresh.png)(Refresh) 아이콘을 클릭하면 작업 중인 PSM 문장 목록이 업데이트된다.

다음은 PSM Editor 화면의 세부 기능에 대한 설명이다.

<figure><img src="../../../../.gitbook/assets/image (65).png" alt="" width="375"><figcaption><p>[그림 1] PSM Editor</p></figcaption></figure>



*   **아이콘**

    다음은 화면의 아이콘에 대한 설명이다.

    | 아이콘                 | 설명                                                         |
    | ------------------- | ---------------------------------------------------------- |
    | PSM Compile         | PSM 문장을 컴파일한다.                                             |
    | PSM Run             | PSM 문장을 실행한다.                                              |
    | PSM Debug           | PSM 문장을 디버그한다. 설정된 Breakpoint가 없을 경우 PSM Run과 같은 동작이 수행된다. |
    | Terminate PSM Debug | 수행 중인 디버거의 연결을 끊는다.                                        |
    | Resume              | 설정된 다음 Breakpoint로 디버그 라인을 이동한다.                           |
    | Step Into           | 디버깅 도중 프러시저를 호출할 경우 호출한 프러시저 안으로 디버깅 라인이 이동한다.             |
    | Step Any Return     | 프러시저 호출부의 다음 라인으로 디버깅 라인을 이동한다.                            |
    | Step Over           | 다음 라인으로 디버그 라인을 이동한다.                                      |
*   **컨텍스트 메뉴**

    Editor 영역에서 오른쪽 마우스 버튼을 클릭하면 PSM 문장을 편집할 때 사용할 수 있는 컨텍스트 메뉴가 나타난다. \
    Compile, Debug, Run 메뉴는 각 PSM 문장을 컴파일하고, 디버그 하고, 실행한다. **Add Variable** 메뉴는 선택한 영역의 텍스트를 Variable Tab에 Variable로 추가한다. Compile, Debug, Run, **Add Variable** 메뉴를 제외한 각 메뉴는  [SQL Editor](../sql-editor/) 컨텍스트 메뉴와 동일하다.

<figure><img src="../../../../.gitbook/assets/image (66).png" alt="" width="375"><figcaption><p>[그림2] PSM Editor Context Menu</p></figcaption></figure>

