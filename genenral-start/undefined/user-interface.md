---
description: 본 장에서는 Tibero Studio의 화면 구성에 대해 설명한다.
---

# User Interface

## User Interface

Tibero Studio를 실행하고 나서 데이터베이스 서버에 접속하면 다음과 같은 초기 화면이 나타난다.

<figure><img src="../../.gitbook/assets/image (86).png" alt=""><figcaption><p>[그림 n.1] 초기화면</p></figcaption></figure>

초기 화면은 5개의 영역으로 구성된다.

*   **① Menu**

    Tibero Studio에서 사용할 수 있는 전체 기능의 메뉴이다. 자세한 설명은 [“화면  세부기능”](user-interface.md#d5e974)를 참고한다.
*   **② Tool bar**

    빠르고 간편하게 메뉴를 실행할 수 있도록 메뉴 중 일부가 아이콘 형태로 나열되어 있다. 자세한 설명은 [“Main Tool bar”](user-interface.md#d5e1596)를 참고한다.
*   **③ Schema Tree Browser**

    Tibero Studio과 연결을 유지하고 있는 데이터베이스의 스키마 객체의 정보가 트리 형태로 나타난다.  Tibero Studio에서 Schema Tree Browser 영역에서는 다음의 기능을 제공한다. 자세한 설명은 ["Schema Tree Browser"](schema-tree-browser/)를 참고한다.

    * Search Object
    * Toolbar
    * GUI Operator
    * Object Property
*   **④ Editor**

    SQL Editor, PSM Editor, Schema Object Detail 및 Developer 기능 관련 정보를 보여준다.

    Tibero Studio에서 View 영역에서 다음의 기능을 제공한다. 자세한 설명은 ["Editor"](editor/)를 참고한다.

    * SQL Editor&#x20;
    * PSM Editor
*   **⑤ ETC**

    그외 Task List, SQL History, Template, Invalid Object Recompile, Exp/Imp 등 다양한 기능을 제공한다. 자세한 설명은 ["ETC"](../../etc/)를 참고한다.&#x20;

## 화면 세부 기능 <a href="#d5e974" id="d5e974"></a>

본 절에서는 화면의 각 부분을 구성하는 세부 기능에 대해서 설명한다.

### Menu <a href="#sect_main_menu" id="sect_main_menu"></a>

Menu는 다음 그림과 같이 총 6개 영역으로 구성된다.

<figure><img src="../../.gitbook/assets/image (85).png" alt=""><figcaption><p>[그림 n.2] Menu</p></figcaption></figure>

### **File**

데이터베이스 서버와의 접속, 파일 불러오기 및 저장, 인쇄 등과 관련된 메뉴이다.

<table><thead><tr><th width="227">메뉴</th><th>설명</th></tr></thead><tbody><tr><td>New Editor </td><td><p>새로운 SQL 혹은  PSM 에디터를 연다. </p><ul><li>SQL Editor : 새로운 SQL Editor를 연다.</li><li>PSM Editor : 새로운 PSM Editor를 연다.</li></ul></td></tr><tr><td>Open File </td><td>저장된 SQL 파일을 SQL Editor에 불러온다.</td></tr><tr><td>Recent Editor</td><td><p>최근에 종료된 에디터를 연다. </p><ul><li>History (1~9) :  최근에 종료된 에디터를 순서대로 보여준다.</li><li>Clear History : 저장된 히스토리 리스트를 지운다.</li></ul></td></tr><tr><td>New Connection</td><td>새로운 커넥션에 접속한다.</td></tr><tr><td>Invalid / Reconnect Connection</td><td>선택된 Connection을 검증/재연결 한다.</td></tr><tr><td>End Connection </td><td>선택된 연결정보를 끊는다.</td></tr><tr><td>End All Connection </td><td>모든 커넥션을 끊는다.</td></tr><tr><td>Session Info </td><td>현재 접속된 세션(Session) 정보를 보여준다</td></tr><tr><td>Change Password</td><td>현재 접속된 사용자의 패스워드를 변경한다.</td></tr><tr><td>Save </td><td>현재 포커스된 SQL Editor의 내용을 저장한다.</td></tr><tr><td>Save as</td><td>현재 열려 있는 SQL Editor의 내용을 다른 이름으로 저장한다.</td></tr><tr><td>Save All</td><td>현재 열려 있는 모든 SQL Editor의 내용을 저장한다.</td></tr><tr><td>Switch Default Folder</td><td>기본 저장 경로를 수정한다.</td></tr><tr><td>Print</td><td>프린터 대화상자를 실행한다.</td></tr><tr><td>Exit</td><td>Tibero Studio를 종료한다.</td></tr></tbody></table>

### **Edit**

Editor 영역에서 SQL 문장을 편집하는 것과 관련된 메뉴이다.

<table><thead><tr><th width="181">메뉴</th><th>설명</th></tr></thead><tbody><tr><td>Undo</td><td>Editor를 사용할 때 잘못된 편집을 취소한다.</td></tr><tr><td>Redo</td><td>Editor를 사용할 때 취소했던 편집이나 실행을 다시 실행한다.</td></tr><tr><td>Cut</td><td>선택된 모든 텍스트를 잘라서 클립보드(clipboard)에 복사한다.</td></tr><tr><td>Copy</td><td>선택된 모든 텍스트를 클립보드에 복사한다.</td></tr><tr><td>Paste</td><td>클립보드에 있는 복사된 텍스트를 Editor에 붙여 넣는다.</td></tr><tr><td>Delete</td><td>커서의 문자를 삭제하거나 선택한 영역 내의 모든 문자를 삭제한다.</td></tr><tr><td>Delete All</td><td>영역 내의 모든 문자를 삭제한다.</td></tr><tr><td>Select All</td><td>Editor에 있는 모든 문자를 선택한다.</td></tr><tr><td>Block Select Mode</td><td>l커서의 문자를 블록형태로 선택한다.</td></tr><tr><td>Find &#x26; Replace</td><td>Editor에 있는 특정 문자를 찾는다.</td></tr><tr><td>Format</td><td><p>비규칙적이고 읽기 어려운 SQL을 보기 좋게 만들어 줌으로써 가독성을 높인다.</p><ul><li>Formatting : 비규칙적이고 읽기 어려운 SQL을 보기 좋게 만들어 줌으로써 가독성을 높인다.</li><li>Format All : 비규칙적이고 읽기 어려운 모든 SQL을 보기 좋게 만들어 줌으로써 가독성을 높인다.</li><li>Trim spaces : 선택한 내의  앞 / 뒤 공백을 삭제한다.선택한 영역내의 앞 / 뒤 공백을 삭제한다.</li><li>Single Line Comments : 선택 영역 내의 라인을 주석으로 처리한다.</li><li>Multi Line Comments : 선택 영역 내의 모든 라인을 주석으로 처리한다.</li><li>Indent : 커서 위치에서 텍스트를 들여쓴다.</li><li>Unindent : 커서 위치에서 텍스트를 내어쓴다.</li></ul></td></tr><tr><td>Convert</td><td><p>문자의 형식을 변경한다.</p><ul><li>Lower case : 선택 영역 내의 모든 문자를 소문자로 변경한다.</li><li>Upper case : 선택 영역 내의 모든 문자를 대문자로 변경한다.</li><li>Capitalize : 선택 영역 내의 모든 단어의 첫 글자는 대문자로 변경하고 나머지 글자는 소문자로 변경한다.</li><li>Sentensize : 선택 영역 내의 모든 문장의 첫 글자는 대문자로 변경하고 나머지 글자는 소문자로 변경한다.</li><li>Invert case : 선택 영역 내의 모든 대문자는 소문자로 변경하고, 소문자는 대문자로 변경한다.</li></ul></td></tr><tr><td>Word Wrap</td><td>Editor 자동 줄 바꿈모드를  변경한다.</td></tr><tr><td>Auto Complete</td><td>커서 위치에서 자동완성창을 호출한다.</td></tr></tbody></table>

### **Run (Action)**

SQL 문장의 실행과 관련된 메뉴이다.

<table><thead><tr><th width="219">메뉴</th><th>설명</th></tr></thead><tbody><tr><td>Run SQL</td><td>선택된 SQL 문이나 다수의 SQL 문을 실행한다.</td></tr><tr><td>Run All From Cursor</td><td>현재 커서부터 끝까지 SQL 문을 실행한다.</td></tr><tr><td>Run Step</td><td>현재 커서에서부터 하나씩 실행하면서 다음 SQL 문으로 이동한다.</td></tr><tr><td>Run SQL Script</td><td>현재 커서에 있는  현재 커서가 있는 문서의 모든 SQL을 수행한다.문을 실행한다.</td></tr><tr><td>Run SQL New Tab</td><td>이전에 수행하였던 SQL 문 수행 결과를 남겨놓고 추가적인 화면으로 보여준다.</td></tr><tr><td>Run Subquery Block</td><td>선택된 SQL의 Subquery를 수행한다.</td></tr><tr><td>Show Execution Plan</td><td>선택된 SQL 문의 실행 계획을 보여준다.</td></tr><tr><td>Show SQL Trace</td><td>실행한 SQL 문에 대한 통계 정보를 보여준다.</td></tr><tr><td>Commit</td><td>쿼리 결과를 데이터에 영구적으로 반영하기 위해서 실행한다.</td></tr><tr><td>Rollback</td><td>지금까지 DML을 실행한 결과를 취소한다.</td></tr><tr><td>Compile</td><td>선택된 PSM을 컴파일 한다.</td></tr><tr><td>Debug</td><td>선택된 PSM의 문장을 디버그 한다.</td></tr><tr><td>Run PSM</td><td>선택된 PSM 문장을 실행한다.</td></tr><tr><td>Append Query Result</td><td>SQL 수행 시 무조건 새로운 탭을 생성하도록 한다.</td></tr></tbody></table>

### **View**

Tibero Studio의 탭과 관련된 메뉴이다.

<table><thead><tr><th width="226">메뉴</th><th>설명</th></tr></thead><tbody><tr><td>Maximize Editor</td><td>Editor 영역을 최대화, Result 영역을 최소화 한다.</td></tr><tr><td>Maximize Result</td><td>Editor 영역을 최소화, Result 영역을 최대화 한다.</td></tr><tr><td>Schema Tree Browser</td><td>접근할 수 있는 사용자의 모든 스키마 정보를 트리 형태로 제공한다.</td></tr><tr><td>Split Vertical</td><td>화면을 세로로 나눠 탭을 분할한다.</td></tr><tr><td>Split Horizontal</td><td>화면을 가로로 나눠 탭을 분할한다.</td></tr><tr><td>Collapse Tab Group</td><td>분할된 탭을 합친다.</td></tr><tr><td>Lock Tabs</td><td>Split View 기능을 막는다</td></tr><tr><td>DBMS Output</td><td>DBMS Output 탭을 연다.</td></tr><tr><td>SQL History</td><td>SQL History 탭을 연다.</td></tr><tr><td>Task List</td><td>Task List 탭을 연다.</td></tr><tr><td>Template</td><td>템플릿 설정 탭을 연다.</td></tr><tr><td>Tools</td><td><ul><li>File Load/Unload : Load와 Unload를 할 수 있는 기능을 제공한다.</li><li>Recompile Invalid Object : 유효하지 않은 객체를 컴파일하는 기능을 제공한다.</li></ul></td></tr><tr><td>Move</td><td><p>탭 포커스를 이동한다.</p><ul><li>Next Tab : 다수의 SQL Editor 탭이 있을 경우 다음 탭으로 포커스를 이동한다.</li><li>Previous Tab : 다수의 SQL Editor 탭이 있을 경우 이전 탭으로 포커스를 이동한다.</li><li>Copy to Next tab : 현재 SQL Editor를 새로운 탭으로 복사한다.</li><li>Go To Tab : Tab 목록에서 탭을 선택하여 해당 탭으로 포커스를 이동한다.</li></ul></td></tr><tr><td>Close Tab</td><td>현재 포커스 된 탭을 닫는다.</td></tr><tr><td>Close All Tab</td><td>모든 탭을 닫는다.</td></tr><tr><td>Close Other</td><td>현재 포커스 된 탭을 제외하고 모든 탭을 종료한다.</td></tr></tbody></table>

### **Window**

Tibero Studio의  Window와 관련된 메뉴다.

<table><thead><tr><th width="238">메뉴</th><th>설명</th></tr></thead><tbody><tr><td>New Window</td><td>새로운 스튜디오 윈도우를 연다.</td></tr><tr><td>Toggle Full Screen</td><td>전체화면으로 전환한다.</td></tr><tr><td>Maximize Window (On / Off)</td><td>창을 최대화 한다.</td></tr><tr><td>Minimize Window</td><td>창을 최소화 한다.</td></tr><tr><td>Preference</td><td>환경설정할 수 있는 Preference 창을 킨다.</td></tr></tbody></table>

### **Help**

Tibero Studio의 버전 정보와 단축키와 관련된 메뉴이다.

| 메뉴         | 설명                               |
| ---------- | -------------------------------- |
| Studo Info | Tibero Studio의 도움말과 버전 정보를 조회한다. |
| Help       | 테크넷 Manual 연결                    |

## Main Tool bar <a href="#d5e1596" id="d5e1596"></a>

빠르고 간편하게 메뉴를 실행할 수 있도록 메뉴 중 일부가 툴바에 표시된다. 툴바의 아이콘을 클릭했을 때 실행되는 메뉴는 다음과 같다.

<table><thead><tr><th width="139">아이콘</th><th>설명</th></tr></thead><tbody><tr><td><img src="https://technet.tmax.co.kr/upload/download/online/tibero/pver-20170425-000001/user-guide/resources/figure_toolbar_1.png" alt=""></td><td><strong>[File] > [New Connection]</strong> 메뉴를 실행한다.</td></tr><tr><td></td><td>[File] > [Invalid / Reconnect] 메뉴를 실행한다.</td></tr><tr><td><img src="https://technet.tmax.co.kr/upload/download/online/tibero/pver-20170425-000001/user-guide/resources/figure_toolbar_2.png" alt=""></td><td><strong>[File] > [End Connection]</strong> 메뉴를 실행한다.</td></tr><tr><td><img src="https://technet.tmax.co.kr/upload/download/online/tibero/pver-20170425-000001/user-guide/resources/figure_toolbar_10.png" alt=""></td><td><strong>[File] > [SQL Editor]</strong> 메뉴를 실행한다.</td></tr><tr><td><img src="https://technet.tmax.co.kr/upload/download/online/tibero/pver-20170425-000001/user-guide/resources/figure_toolbar_12.png" alt=""></td><td><strong>[File] > [PSM Editor]</strong> 메뉴를 실행한다.</td></tr><tr><td><img src="https://technet.tmax.co.kr/upload/download/online/tibero/pver-20170425-000001/user-guide/resources/figure_toolbar_7.png" alt=""></td><td><strong>[File] > [Open File...]</strong> 메뉴를 실행한다.</td></tr><tr><td><img src="https://technet.tmax.co.kr/upload/download/online/tibero/pver-20170425-000001/user-guide/resources/figure_toolbar_8.png" alt=""></td><td><strong>[File] > [Save]</strong> 메뉴를 실행한다.</td></tr><tr><td><img src="https://technet.tmax.co.kr/upload/download/online/tibero/pver-20170425-000001/user-guide/resources/figure_toolbar_9.png" alt=""></td><td><strong>[File] > [Save as...]</strong> 메뉴를 실행한다.</td></tr><tr><td><img src="https://technet.tmax.co.kr/upload/download/online/tibero/pver-20170425-000001/user-guide/resources/figure_toolbar_5.png" alt=""></td><td><strong>[Run] > [Commit]</strong> 메뉴를 실행한다.</td></tr><tr><td><img src="https://technet.tmax.co.kr/upload/download/online/tibero/pver-20170425-000001/user-guide/resources/figure_toolbar_6.png" alt=""></td><td><strong>[Run] > [Rollback]</strong> 메뉴를 실행한다.</td></tr><tr><td><img src="https://technet.tmax.co.kr/upload/download/online/tibero/pver-20170425-000001/user-guide/resources/figure_toolbar_29.png" alt=""></td><td>[View] > [Tool] > [Compile Invalid Objects] 메뉴를 실행한다.</td></tr><tr><td></td><td>[Window] > [Preference] 메뉴를 실행한다.</td></tr><tr><td></td><td>[File] > [Session Info] 메뉴를 실행한다.</td></tr><tr><td></td><td>[Help] > [Help] 메뉴를 실행한다.</td></tr></tbody></table>

#### 참고

각 메뉴에 대한 자세한 내용은 [“2.2.1. Menu”](https://technet.tmax.co.kr/upload/download/online/tibero/pver-20170425-000001/user-guide/chapter02.html#sect\_main\_menu)와 [“제3장 기본 기능”](https://technet.tmax.co.kr/upload/download/online/tibero/pver-20170425-000001/user-guide/chapter03.html), [“제4장 DBA 기능”](https://technet.tmax.co.kr/upload/download/online/tibero/pver-20170425-000001/user-guide/chapter04.html), [“제5장 개발자 기능”](https://technet.tmax.co.kr/upload/download/online/tibero/pver-20170425-000001/user-guide/chapter05.html)을 참고한다.개요
