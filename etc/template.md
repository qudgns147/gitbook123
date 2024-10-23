# Template

## User Interface

Editor > Context Menu > Template 혹은  GNB > View > Template 을 선택하면 Template 창이 우측에 나타난다.&#x20;

Template 화면의 UI는 다음과 같다.

<figure><img src="../../../.gitbook/assets/image (144).png" alt="" width="375"><figcaption><p>Template</p></figcaption></figure>

Template 창에서는 SQL / PSM 문장을 쉽게 작성할 수 있도록 문장을 저장하고 사용할 수 있다. 또한 Code Template을 통해 사용자가 정의한 다양한 템플릿을 사용자가 정의한 코드를 자동완성을 통해 간편하게 불러올 수 있다.&#x20;

### Toolbar

* **New Template**\
  Template 창에서 \[+ New Template]을 선택하면 다음과 같은 템플릿 추가 창이 열린다.

<figure><img src="../../../.gitbook/assets/image (145).png" alt="" width="375"><figcaption><p>New Template</p></figcaption></figure>

각항목에 대한 자세한 설명은 다음과 같다.

<table><thead><tr><th width="149">항목</th><th>설명</th></tr></thead><tbody><tr><td>Name</td><td>Template의 이름을 정의할 수 있으며, 최대 50자까지 입력 가능하며 중복할 수 없다</td></tr><tr><td>Type</td><td>SQL / PSM / User Defined Code 가 있으며  User Defined Code의 경우 해당 이름을 기준으로 자동완성을 할 수 있다.</td></tr><tr><td>Code</td><td>입력할 Code를 정의할 수 있다. 하단 Variables 선택 시 자동입력  될 변수를 선택할 수 있다. 각 변수는 자동완성 후 해당 변수를 바로 편집하도록 정의한다.</td></tr><tr><td>Add</td><td>Template 목록에 Template을 추가한다.</td></tr></tbody></table>

* **Reset**\
  Template List를 애플리케이션 초기 상태로 되돌릴 수 있다. 이전에 추가한 Template들이 삭제되고 되돌릴 수 없기 때문에 주의해서 사용해야 한다.

### Template List

저장된 정보는 Template List는 해당 리스트 더블 클릭을 통해 현재 Editor에 입력된다. 또한 User Defined Code의 경우 Template 이름을 기준으로 자동완성된다.

해당 리스트에서 Context Menu를 통해 Template 정보를 추가 / 삭제 / 편집이 가능하다.&#x20;

### Code Preview

현재 선택된 Template의 Code를 보여준다.&#x20;

Code Formating을 활성화하면 사용자 정의와 관계 없이 현재 코드에 대한 Formating한 상태로 Code가 입력된다.&#x20;
