---
description: 'Run / Trace / Plan : 수행 내용 포함'
---

# SQL Editor 영역

Editor 영역에서 SQL 문장을 입력, 편집, 실행하고 저장할 수 있다.

### **SQL 문장의 입력과 편집**

Editor 영역에서 SQL 문장을 입력하고 편집하는 방법은 다음과 같다.

*   일반적인 SQL 문장의 입력

    일반적인 SQL 문장은 Editor 영역에 입력하며, 하나의 SQL 문장을 여러 라인에 걸쳐 입력할 수 있다.

    여러 라인에 걸쳐 입력할 경우 하나의 SQL 문장을 한 라인의 연속된 문자열 형태가 아닌 여러 라인으로 분리된 형태로 입력할 수 있다. 대부분 절 단위로 분리하여 입력하는데, 이렇게 절 단위로 분리해서 입력하면 읽기가 편하고 변경이 쉽다.
*   템플릿을 사용한 SQL 문장의 입력

    **Context Menu > \[Template]** 메뉴를 선택하거나 View > Template 을 클릭하면 SQL 및 PSM과 Code 문장을 작성해 두어 쉽게 사용하기 위한 탭이 나타난다. 트리 형태로 나타난 각 템플릿의 이름을 더블클릭하면 Editor 영역에 해당 문장의 템플릿이 입력된다. 입력된 템플릿을 수정하여 손쉽게 SQL 문장을 완성할 수 있다.
*   주석(comment)의 삽입

    SQL 문장을 입력하는 중간에 주석을 삽입할 수 있다. 주석은 두 개의 마이너스 기호(−−)로 시작되며, 그 라인의 마지막까지 주석으로 포함한다. 주석은 자체만으로 하나의 라인이 될 수도 있으며, 한 라인에서 다른 문자열의 뒤쪽에 위치할 수도 있다.
*   단축키의 사용

    기존의 다른 Text Editor와 마찬가지로 다시 실행(\<Ctrl> + Y), 실행 취소(\<Ctrl> + Z), 찾기/바꾸기(\<Ctrl> + F) 단축키를 제공한다.

### **SQL 문장의 실행**

Editor 영역에서 SQL 문장을 실행하는 방법은 다음과 같다.

*   여러 SQL 문장의 실행

    SQL 문장을 실행할 때 해당 Editor 영역의 모든 SQL 문장을 실행( Run Script)하거나 선택한 문장(Run SQL)을 실행할 수 있다. 여러 SQL 문장을 실행했을 경우 화면 하단의 Result View에 각 SQL 문장마다 탭이 생성되며 각각의 결과를 개별적으로 확인할 수 있다.
*   Task List\
    Editor에서 Task는 실행 단위를 의미한다. Editor 영역에 SQL을 작성하고 실행했을 때 작성한 SQL을 포함하는 Task 하나가 생성이 된다.

    SQL을 실행했을 경우 Task List 영역에 실행중인 혹은 실행 대기중인 Task List가 나타나고, Task 선택 후 (Delete) 아이콘을 클릭하면 실행 중인 Task 가 실행 취소되고 다음 Task 실행으로 넘어간다.

    각 Task row를 클릭하면 Task에서 실행될 SQL들을 확인할 수 있다.
*   여러 SQL 문장 실행에서 에러 처리

    여러 SQL 문장 실행에서 에러가 발생했을 경우 에러 화면이 나타난다.

\


<figure><img src="../../../../.gitbook/assets/image (102).png" alt="" width="215"><figcaption><p>Error 처리</p></figcaption></figure>

에러 발생 시, 선택에 따라 에러를 스킵하고 이후 쿼리들을 실행할 수 있다. **\[Stop Running Task] 버튼**을 클릭하면 에러가 발생한 쿼리 이후의 쿼리들을 실행하지 않는다.

| 선택 항목                             | 설명                                                                  |
| --------------------------------- | ------------------------------------------------------------------- |
| **Applicable to Only this Error** | 현재 에러가 발생한 SQL에 대해서만 건너뛰고 다음 SQL을 실행한다.                             |
| **Applicable to All Same Errors** | 현재 발생한 에러와 동일한 JDBC Number의 에러가 발생 할 시 모두 건너뛰고 이외의 SQL은 정상적으로 실행한다. |
| **Applicable to All Errors**      | 이후 에러가 발생하는 모든 SQL문을 건너 뛴다.                                         |

* Bind Parameter

<figure><img src="../../../../.gitbook/assets/image (103).png" alt="" width="375"><figcaption><p>[그림 n.4]  Bind Parameter</p></figcaption></figure>

변수가 있는 쿼리를 실행하였을 경우, 변수에 값을 할당하는 **Bind Variable 화면**이 나타난다.

<table><thead><tr><th width="188">항목</th><th>설명</th></tr></thead><tbody><tr><td>Name</td><td>바인드 변수 이름을 나타낸다.</td></tr><tr><td>Data Type</td><td>바인드 변수의 데이터 타입을 나타낸다.</td></tr><tr><td>Value</td><td>바인드 변수에 삽입할 값을 입력한다.</td></tr><tr><td>Hide parameters set in script</td><td>값을 실제 스크립트에 변환하여 삽입할지 여부를 나타낸다.</td></tr></tbody></table>



