---
description: SQL Editor의 UI와 Toolbar에 대해 설명한다.
---

# SQL Editor

메인 화면에서 **\[File] > \[New Editor] > \[SQL Editor]** 메뉴를 선택하거나 Tab 영역의 \[+버튼]  > \[SQL Editor]를  클릭하면 **SQL Editor 화면**이 나타난다. SQL Editor에서는SQL 문장을 입력하고 저장할 수 있으며, SQL 문장의 실행 계획(Execution Plan)을 확인할 수 있다. 또한 초보자도 쉽게 SQL 문장을 작성할 수 있도록 템플릿도 제공된다.

**SQL Editor 화면**은 SQL 문장을 입력하고 실행할 수 있는 화면 상단의 **Editor 영역**과 SQL 문장의 실행 결과나 실행 계획을 볼 수 있는 화면 하단의 Result View 영역으로 구성된다.

다음은 SQL Editor 화면의 세부 기능에 대한 설명이다.

<figure><img src="../../../../.gitbook/assets/image (100).png" alt="" width="375"><figcaption><p>[그림n.1] SQL Editor</p></figcaption></figure>

*   **아이콘**

    <table><thead><tr><th width="140">아이콘</th><th>설명</th></tr></thead><tbody><tr><td>Run SQL </td><td><p>선택된 SQL 문이나 다수의 SQL 문을 실행한다.</p><p><strong>[Run] > [Run SQL]</strong> 메뉴에 대한 단축 아이콘이다.</p></td></tr><tr><td>Run Script</td><td><p>현재 Editor의  처음부터 끝까지 SQL 문을 실행한다.</p><p><strong>[Run] > [Run Script]</strong> 메뉴에 대한 단축 아이콘이다.</p></td></tr><tr><td>Execution Plan</td><td><p>선택된 SQL 문이나 다수의 SQL 문에 대한 실행 계획을 화면 하단에 보여준다.</p><p><strong>[Run] > [</strong>Execution Plan<strong>]</strong> 메뉴에 대한 단축 아이콘이다.</p></td></tr><tr><td>SQL Trace</td><td><p>실행한 SQL 문에 대한 통계 정보를 화면 하단에 보여준다.</p><p><strong>[Run] > [SQL Trace]</strong> 메뉴에 대한 단축 아이콘이다.</p></td></tr><tr><td>SQL History</td><td><p>이전에 실행하였던 SQL 문장들을 다시 확인할 수 있다.</p><p><img src="https://technet.tmax.co.kr/upload/download/online/tibero/pver-20170425-000001/user-guide/resources/figure_sql_history.png" alt=""> 아이콘을 클릭하면, SQL 문장 목록을 보여주는 <strong>[SQL History]</strong> View가 화면 아래쪽에 나타난다.</p></td></tr><tr><td>Commit</td><td><p>DML 실행 후의 결과를 데이터에 영구적으로 반영하기 위해서 실행한다.</p><p><strong>[Run] > [Commit]</strong> 메뉴에 대한 단축 아이콘이다.</p></td></tr><tr><td>Rollback</td><td><p>지금까지 DML을 실행한 결과를 취소한다.</p><p><strong>[Run] > [Rollback]</strong> 메뉴에 대한 단축 아이콘이다.</p></td></tr><tr><td>Commit Setting</td><td>Commit되지 않은 Transaction 리스트 조회 및 Commit 모드를 설정한다.</td></tr></tbody></table>
*   **컨텍스트 메뉴(Context Menu)**

    Editor 영역에서 오른쪽 마우스 버튼을 클릭하면 SQL 문장을 편집할 때 사용할 수 있는 컨텍스트 메뉴가 나타난다.

<figure><img src="../../../../.gitbook/assets/image (101).png" alt="" width="375"><figcaption><p>[그림n.2] SQL Editor Context Menu</p></figcaption></figure>

<table><thead><tr><th width="222">메뉴</th><th>설명</th></tr></thead><tbody><tr><td>Describe</td><td>선택한 영역의 객체에 대한 Describe 화면을 연다.</td></tr><tr><td>Run SQL</td><td><p>선택된 SQL 문이나 다수의 SQL 문을 실행한다.</p><ul><li>Run SQL : 선택된 SQL 문이나 다수의 SQL 문을 실행한다.</li><li>Run All From Cursor : 현재 커서부터 끝까지 SQL 문을 실행한다.</li><li>Run Step : 현재 커서부터 하나씩 실행하면서 다음 SQL 문으로 이동한다.</li><li>Run SQL Script : 현재 Editor Tab에 있는 전체 SQL 실행한다.</li><li>Run SQL NewTab : 새로운 결과 창으로 SQL 실행한다.</li><li>하위 쿼리 블록 실행 : 하위 쿼리(SubQuery)만 실행한다.</li></ul></td></tr><tr><td>Execute Plan</td><td>선택된 SQL 문이나 다수의 SQL 문에 대한 실행 계획을 화면 하단에 보여준다.</td></tr><tr><td>Copy</td><td>선택한 영역을 복사한다.</td></tr><tr><td>Cut</td><td>선택한 영역을 잘라낸다.</td></tr><tr><td>Paste</td><td>복사한 내용을 붙인다.</td></tr><tr><td>Select All</td><td>모든 내용을 선택한다.</td></tr><tr><td>Undo</td><td>실행을 취소한다.</td></tr><tr><td>Redo</td><td>취소한 실행을 다시 실행한다.</td></tr><tr><td>Format</td><td><p>비규칙적이고 읽기 어려운 SQL을 보기 좋게 만들어 줌으로써 가독성을 높인다.</p><ul><li>Format : 비규칙적이고 읽기 어려운 SQL을 보기 좋게 만들어 줌으로써 가독성을 높임</li><li>Trim spaces : 커서가 있는 행, 혹은 선택한 행의 처음과 끝에 있는 공백 삭제한다.</li><li>Word Wrap : 현재 Layout 크기에 맞게 자동으로 줄바꿈 한다.</li><li>Single Line Comments : 해당 커서가 있는 행을 한줄 주석 처리한다.</li><li>Multi Line Comments : 해당 블록 앞과 뒤에 /*, */ 삽입하여 블록을 주석처리 한다.</li></ul></td></tr><tr><td>Convert Case</td><td><p>비규칙적이고 읽기 어려운 모든 SQL을 보기 좋게 만들어 줌으로써 가독성을 높인다.</p><ul><li>Upper case : 모든 단어를 대문자로 변경한다.</li><li>Lower case : 모든 단어를 소문자로 변경한다.</li><li>Capitalize : 모든 단어의 첫 글자를 대문자로 변경한다.</li><li>Invert case : 대문자는 소문자로, 소문자는 대문자로 변경한다.</li></ul></td></tr><tr><td>Template</td><td>사용자가 정의한 Template List를 볼 수 있는 탭을 연다.</td></tr><tr><td>Save</td><td>현재 포커스된 SQL Editor의 내용을 저장한다.</td></tr><tr><td>Preference</td><td>환경설정을 할 수 있는 Preference 창을 연다.</td></tr></tbody></table>
