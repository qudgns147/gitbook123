---
description: >-
  PSM Editor의 Result View 영역에서는 DBMS Output, Breakpoint List, Variable,
  Backtrace, Error 탭을 통해 PSM 수행과 관련한 정보를 조회할 수 있다.
---

# Result View 영역

## Result View <a href="#d5e3133" id="d5e3133"></a>

Result View 영역에서 해당 PSM 문장의 실행 결과를 볼 수 있다. Editor 영역에 PSM 문장을 입력하고 **PSM Editor 화면**([\[그림 3.17\]](https://technet.tmax.co.kr/upload/download/online/tibero/pver-20230906-000001/user-guide/chapter03.html#figure\_psmeditor\_full) 상단에 위치한 **\[Compile] 버튼**을 클릭하면 컴파일이 되고, **\[Run] 버튼**을 클릭하면 PSM Editor 화면 하단에 위치한 View 영역에 해당 PSM 문장의 실행 결과가 나타난다.



### DBMS Output 탭

PSM 문장을 실행한 결과가 표시된다. PSM 문장을 실행할 때 에러가 발생하면 이 탭에 에러 메시지가 표시된다.&#x20;

<figure><img src="../../../../.gitbook/assets/image (111).png" alt="" width="375"><figcaption><p>[그림 n.1] DBMS Output</p></figcaption></figure>

\
\[Save as File] 버튼을 통해 .txt 파일로 저장할 수 있고, Clear 버튼을 통해 모든 Text 데이터를 지울 수 있다. \[Move To Last Line] 설정을 통해 마지막 줄로 자동 스크롤 한다.



### Breakpoint List 탭

설정된 Breakpoint의 목록을 조회할 수 있다.

<figure><img src="../../../../.gitbook/assets/image (113).png" alt="" width="375"><figcaption><p>[그림 n.2] Breakpoint List 탭</p></figcaption></figure>

Breakpoints에서 나타나는 정보에 대한 자세한 설명은 다음과 같다.

<table><thead><tr><th width="205">항목</th><th>설명</th></tr></thead><tbody><tr><td>Location</td><td>Breakpoint 가 설정된 PSM Editor를 나타낸다.</td></tr><tr><td>Line</td><td>PSM Editor의 Breakpoint Line을 의미한다.</td></tr><tr><td>Status</td><td>해당 Breakpoint를 사용하는지 여부를 나타낸다.</td></tr><tr><td>Description</td><td>Breakpoint에 대한 설명을 작성할 수 있다.</td></tr></tbody></table>



### Variables 탭

디버깅 중 클래스에 해당하는 변수와 데이터 값의 리스트를 조회할 수 있다.\
모든 변수 중 일부를 Watch로 설정하여 디버그 수행에 따라 변하는 값을 확인할 수 있다.&#x20;

<figure><img src="../../../../.gitbook/assets/image (114).png" alt="" width="375"><figcaption><p>[그림 n.3] Variables Tab - Variable</p></figcaption></figure>

각 항목에 대한 설명은 다음과 같다.

<table><thead><tr><th width="213">항목</th><th>설명</th></tr></thead><tbody><tr><td>Watch</td><td>감시 여부에 대해 설정한다.</td></tr><tr><td>Name</td><td>Variable의 이름을 나타낸다</td></tr><tr><td>Value</td><td>현재 Variable의 값을 나타낸다.</td></tr><tr><td>Type</td><td>Variable의 타입을 나타낸다.</td></tr><tr><td>+Add Variable</td><td>Variable 값을 사용자가 직접 추가한다.</td></tr></tbody></table>

<figure><img src="../../../../.gitbook/assets/image (115).png" alt="" width="375"><figcaption><p>[그림 n.4] Variables Tab - Watch list</p></figcaption></figure>

각 항목에 대한 설명은 다음과 같다.

| 항목             | 설명                    |
| -------------- | --------------------- |
| Watch          | 감시 여부에 대해 나타낸다.       |
| Name           | Variable의 이름을 나타낸다    |
| Value          | 현재 Variable의 값을 나타낸다. |
| Type           | Variable의 타입을 나타낸다.   |
| Previous Value | 현재 값의이전 값을 나타낸다.      |

### Backtrace 탭

디버그 수행 중인 PSM 문장의 스택을 확인할 수 있다.\
수행 중인 오브젝트가 몇 번째 줄에서 호출되었는지 확인할 수 있다.

<figure><img src="../../../../.gitbook/assets/image (116).png" alt="" width="375"><figcaption><p>[그림 n.5] Backtrace Tab</p></figcaption></figure>



### Error 탭

PSM 문장 Debug, Compile, Run 수행 시 발생한 모든 에러를 표시한다. 각 항목을 클릭하면 에러가 발생한 위치로 이동한다.&#x20;

<figure><img src="../../../../.gitbook/assets/image (117).png" alt="" width="375"><figcaption><p>[그림 n.7] Error 탭</p></figcaption></figure>

PSM 수행 중 발생한 모든 Error 리스트를 보여주며, Error 선택 후 \[Go to Error]를 통해 해당 에러의 위치로 이동할 수 있다.

