---
description: PSM 문장 입력과 Execute / Debug / Compile 포함 실행에 대해 설명한다.
---

# PSM Editor 영역

#### &#x20;Editor <a href="#d5e3038" id="d5e3038"></a>

Editor 영역에서 PSM 문장을 입력, 편집, 실행하고 저장할 수 있다.

### **PSM 문장의 입력과 편집**

<figure><img src="../../../../.gitbook/assets/image (106).png" alt="" width="375"><figcaption><p>[그림 n.1] PSM Editor</p></figcaption></figure>

Editor 영역에서 PSM 문장을 입력하고 편집하는 방법은 다음과 같다.

*   일반적인 PSM 문장의 입력

    일반적인 PSM 문장은 Editor 영역에 입력하며, 하나의 PSM 문장을 여러 라인에 걸쳐 입력할 수 있다.

    여러 라인에 걸쳐 입력할 경우 하나의 PSM 문장을 한 라인의 연속된 문자열 형태가 아닌 여러 라인으로 분리된 형태로 입력할 수 있다. 대부분 절 단위로 분리하여 입력하는데, 이렇게 절 단위로 분리해서 입력하면 읽기가 편하고 변경이 쉽다.
*   템플릿을 사용한 PSM 문장의 입력

    **Context Menu > \[Template]** 메뉴를 선택하거나 View > Template 을 클릭하면 SQL 및 PSM과 Code 문장을 작성해 두어 쉽게 사용하기 위한 탭이 나타난다. 트리 형태로 나타난 각 템플릿의 이름을 더블클릭하면 Editor 영역에 해당 문장의 템플릿이 입력된다. 입력된 템플릿을 수정하여 손쉽게 PSM 문장을 완성할 수 있다.
*   주석의 삽입

    PSM 문장을 입력하는 중간에 주석을 삽입할 수 있다. 주석은 두 개의 마이너스 기호(−−)로 시작되며, 그 라인의 마지막까지 주석으로 포함한다. 주석은 자체만으로 하나의 라인이 될 수도 있으며, 한 라인에서 다른 문자열의 뒤쪽에 위치할 수도 있다.
*   단축키의 사용

    기존의 다른 텍스트 Editor와 마찬가지로 다시 실행(\<Ctrl> + Y), 실행 취소(\<Ctrl> + Z), 찾기/바꾸기(\<Ctrl> + F) 단축키를 제공한다.

### **PSM 문장의 컴파일 실행과 저장**

Editor 영역에서 PSM 문장을 컴파일하고실행하고 저장하는 방법은 다음과 같다.

<figure><img src="../../../../.gitbook/assets/image (108).png" alt="" width="375"><figcaption><p>[그림 n.2] PSM Compile</p></figcaption></figure>

* PSM 문장의 컴파일\
  PSM 문장을   Compile ( ) 한다.  PSM 문장이  비정상적일 경우 Invalid Object로 저장된다.&#x20;
*   PSM 문장의 실행

    PSM Compile(  )하여, PSM 문장이 성공적으로 컴파일되는지 확인한다. 성공적으로 컴파일되면 PSM Run(  )을 실행하여 PSM 문장을 실행한다.
*   PSM 문장의 저장과 Editor의 탭 이름 변경

    PSM 문장의 저장(   )은 PSM Editor의 탭을 기준으로 저장하며, 기존의 PSM 파일을 불러온 경우 Editor의 탭 이름은 파일명으로 바뀐다.

### **PSM 디버거의 실행**

Editor 영역에서 PSM 문장을 디버그하는 방법은 다음과 같다.

<figure><img src="../../../../.gitbook/assets/image (109).png" alt="" width="375"><figcaption><p>[그림 n.3] PSM Debug</p></figcaption></figure>

*   문장 입력

    디버그할 PSM 문장을 Editor에 입력한다.
*   Breakpoint 설정

    라인 번호의 오른쪽을 클릭하면 해당 라인에 Breakpoint가 설정된다. PSM 디버그가 실행되면 PSM 문장에 설정 가능한 Breakpoint만 남는다.
* Debug Compile\
  디버그를 위한 컴파일을 수행한다.&#x20;
* Debug Run\
  Editor 상단 탭에 PSM Debug로 디버그를 시작한다.&#x20;
*   Variable 설정

    디버깅 중 값의 변화를 추적하고 싶은 variable이 있다면 다음과 같은 방법으로 추적할 수 있다.

    PSM Editor에 작성된 PSM 문에서 원하는 variable name을 선택한 후 마우스 우클릭을 통해 컨텍스트 메뉴를 띄워 Add variable을 클릭하면 variable 리스트에 등록할 수 있다.
*   디버그 진행

    &#x20;**\[Resume]**, \[Step Into], \[Step Any Return], **\[Step Over]** 버튼으로 PSM 디버거를 진행한다.
*   디버그 완료

    디버그가 완료되면 수행한 PSM의 결과를 볼 수 있다.  또한Terminate 버튼으로 PSM 디버그 중 디버그를 중지할 수 있다.

### **Package/Package Body 디버깅 방법**

Editor 영역에서 Package/Package Body 문장을 디버그하는 방법은 다음과 같다.

<figure><img src="../../../../.gitbook/assets/image (110).png" alt="" width="375"><figcaption><p>[그림 n.4] Package Debug</p></figcaption></figure>

* PSM 호출문 생성
  * Package를 Compile하여 생성한 후 Subprogram list 영역에 Package 내에 존재하는P Procedure/Function을 세팅한다.
  * Package가 정상적으로 Compile 된 것을 확인한 후 Package Body문을 작성한다.
  * 디버깅 할 프로그램 문장에 브레이크 포인트를 설정한다. (반드시 하나 이상의 브레이크 포인트를 설정해야 한다.)
  * Subprogram list 영역에서 디버그 작업을 진행 할 Procedure나 Function을 하나 선택해 오른쪽 마우스를 클릭한다.
* PSM 디버그
  * PSM 호출문에서 디버깅을 시작한다. PSM Editor toolbar의 ![](https://technet.tmax.co.kr/upload/download/online/tibero/pver-20170425-000001/user-guide/resources/figure\_psm\_tool2-1.png)(PSM Debug) 아이콘을 클릭하여 실행한다. 실행할 때 PSM 호출문 첫 라인으로 디버깅 라인이 이동한다.
