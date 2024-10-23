---
description: 사용자가 Query를 작성하고 편집할 수 있는 Editor 사용방법에 대해 설명한다.
---

# Editor

본 장에서는 사용자가 주로 사용하는 Editor에 대해 설명한다. View는 Studio 화면을 분할하여 사용할 수 있으며, 개별의 Tab 리스트를 갖을 수 있다.

Editor는 SQL Editor와 PSM Editor가 있으며, 각 에디터 별로 SQL 작성 및 실행과 PSM 작성 및 실행에 특화되어 있다. 자세한 설명은  [SQL Editor](sql-editor/)와 [PSM Editor](psm-editor/)에서 확인할 수 있다.

모든 Editor에서는 쿼리 및 코드를 작성할 수 있으며 편집할 수 있다. 이와 관련된 자세한 설명은 다음과 같다.

* 편집과 관련된 공통기능과 설명은 다음과 같다.

<table><thead><tr><th width="184">항목</th><th>설명</th></tr></thead><tbody><tr><td>Undo</td><td>실행을 취소한다.</td></tr><tr><td>Redo</td><td>취소한 실행을 다시 실행한다.</td></tr><tr><td>Cut</td><td>선택한 영역을 잘라낸다.</td></tr><tr><td>Copy</td><td>선택한 영역을 복사한다.</td></tr><tr><td>Paste</td><td>복사한 내용을 붙인다.</td></tr><tr><td>Delete</td><td>선택한 영역을 지운다.</td></tr><tr><td>Delete All</td><td>현재 Editor의 모든 내용을 지운다.</td></tr><tr><td>Select All</td><td>모든 내용을 선택한다.</td></tr><tr><td>Drag/Drop</td><td>Schema Tree에서 객체 이름을 드래그하여 붙여 넣을 수 있다.</td></tr><tr><td>Find &#x26; Replace</td><td>에디터에 Focus 된 상태에서 &#x3C;Ctrl + F> 키를 누르면 검색 창이 나타난다. 검색 창에서 특정 문자열을 검색할 수 있고 다른 문자열로 대체할 수도 있다.</td></tr><tr><td>Format</td><td><p>비규칙적이고 읽기 어려운 SQL을 보기 좋게 만들어 줌으로써 가독성을 높인다.</p><ul><li>Format : 비규칙적이고 읽기 어려운 SQL을 보기 좋게 만들어 줌으로써 가독성을 높임</li><li>Trim spaces : 커서가 있는 행, 혹은 선택한 행의 처음과 끝에 있는 공백 삭제한다.</li><li>Word Wrap : 현재 Layout 크기에 맞게 자동으로 줄바꿈 한다.</li><li>Single Line Comments : 해당 커서가 있는 행을 한줄 주석 처리한다.</li><li>Multi Line Comments : 해당 블록 앞과 뒤에 /*, */ 삽입하여 블록을 주석처리 한다.</li></ul></td></tr><tr><td>자동입력</td><td>여는 괄호 및 따옴표, 쌍따옴표 작성시 닫는 표시 또한 같이 입력된다.</td></tr></tbody></table>

* Editor의 공통기능과 자세한 설명은 다음과 같다.

<table><thead><tr><th width="191">항목</th><th>설명</th></tr></thead><tbody><tr><td>Editor Connection</td><td>각 Editor별 커넥션을 설정한다.</td></tr><tr><td>Error Highlighting</td><td>에러 발생 시 해당 위치에 에러를 표시한다.</td></tr><tr><td>Parameters</td><td>변수가 있는 쿼리를 실행하였을 경우, 변수에 값을 할당하는 Bind Variable 화면이 나타난다</td></tr><tr><td>Highlight</td><td><p>다양한 Highlight 기능 및 편집 기능을 제공한다.</p><p>선택한 텍스트와 동일한 텍스트에 Highlight</p><p>열기, 닫기 괄호 Highlight</p><p>열 편집 : 열 모양으로 선택하여 편집한다.</p><p> </p></td></tr></tbody></table>

* 행번호 영역의 공통기능은 다음과 같다.

<table><thead><tr><th width="196">항목</th><th>설명</th></tr></thead><tbody><tr><td>Line Number</td><td>행 번호 표시 더블 클릭 시 해당 줄을 선택한다.</td></tr><tr><td>Folding</td><td>명령문의 첫 줄을 제외하고 마지막까지</td></tr><tr><td>Bind Parameter</td><td>변수가 있는 쿼리를 실행하였을 경우, 변수에 값을 할당하는 Bind Parameter 화면이 나타난다</td></tr><tr><td>Highlight</td><td><p>다양한 Highlight 기능 및 편집 기능을 제공한다.</p><p>선택한 텍스트와 동일한 텍스트에 Highlight</p><p>열기, 닫기 괄호 Highlight</p><p>열 편집 : 열 모양으로 선택하여 편집한다.</p><p> </p></td></tr></tbody></table>

