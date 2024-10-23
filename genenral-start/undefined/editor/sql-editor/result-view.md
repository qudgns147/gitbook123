---
description: Result View 영역은 해당 SQL 문장의 실행 결과나 실행 계획을 볼 수 있다.
---

# Result View 영역

## **SQL 문장의 실행 결과**

Editor 영역에 SQL 문장을 입력하고 **SQL Editor 화면** 상단에 위치한 (Run) 아이콘을 클릭하거나 Ctrl + Enter 키를 누르면 다음과 같이 화면 하단에 위치한 View 영역에 해당 SQL 문장의 실행 결과가 나타난다.

### Statistics

SQL 문장을 실행하였을 경우, Statistics 탭이 나타난다. Statistics 탭에는 Task 실행 요약 정보 및 수행 완료, 실패 메시지를 보여준다.

<figure><img src="../../../../.gitbook/assets/image (67).png" alt="" width="375"><figcaption><p>[그림 n.1] Statistics </p></figcaption></figure>

### DBMS Output

DBMS Output 탭에서는 DBMS Output을 발생시킬 경우 서버 출력내용을 보여준다.&#x20;

<figure><img src="../../../../.gitbook/assets/image (72).png" alt="" width="375"><figcaption><p>[그림2] DBMS Output</p></figcaption></figure>

### Result Grid

데이터를 조회하는실  SQL을 실행하였을 경우 Result Grid 창이 나타난다. Result Grid 창에서는 각 결과값을 조회/편집이 가능하며, 이를 위한 다양한 Tool을 상/하단에 제공한다.&#x20;

<figure><img src="../../../../.gitbook/assets/image (105).png" alt="" width="375"><figcaption><p>[그림 n.1] Result 화면</p></figcaption></figure>

* **Grid - 상단툴바**

<table><thead><tr><th width="207">항목</th><th>설명</th></tr></thead><tbody><tr><td>SQL Statement</td><td>수행한 SQL을 표시한다.</td></tr><tr><td>Consol Detach</td><td>수행한 쿼리문을 에디터 탭으로 분리한다.</td></tr><tr><td>Result SQL History</td><td>현재 Result Tab에서 수행한 SQL 목록을 볼 수 있다.</td></tr><tr><td>+Where</td><td>수행한 Query 결과에 조건절을 덧붙여 조회한다.</td></tr><tr><td>SQL Filter History</td><td>조건절에 대한 히스토리를 볼 수 있다.</td></tr><tr><td>Customize Filter</td><td>사용자 정의를 통해 결과 테이블 조회 조건을 설정한다.</td></tr></tbody></table>

* Grid - 하단 툴바

<table><thead><tr><th width="219">항목</th><th>설명</th></tr></thead><tbody><tr><td>Rows per Page</td><td>페이지 별 Row의 개수를 설정한다.</td></tr><tr><td>Total N Item</td><td>전체 Row의 수를 의미한다.</td></tr><tr><td>Page 이동 버튼</td><td>각 페이지를 이동한다.</td></tr><tr><td>Refresh</td><td>실행 결과를 새로고침 한다.</td></tr><tr><td>Save</td><td>사용자가 수정한 결과를 실행한다.</td></tr><tr><td>Cancel</td><td>사용자가 수정한 결과를 취소한다.</td></tr><tr><td>(Cell Edit)</td><td>결과 셀을 수정한다.</td></tr><tr><td>(Add Row)</td><td>선택된 셀 하단에 Row를 추가한다.</td></tr><tr><td>(Copy Row)</td><td>하단에 동일한 값의 Row를 추가한다.</td></tr><tr><td>(Delete Row)</td><td>결과 Row를 삭제한다.</td></tr><tr><td>(First Record)</td><td>가장 처음 Row로 이동한다.</td></tr><tr><td>(Last Record)</td><td>가장 마지막 Row로 이동한다.</td></tr><tr><td>Export</td><td>실행 결과를 CSV, txt, SQL 파일 등으로 추출한다.</td></tr><tr><td>Fetch All</td><td>전체 데이터를 미리 불러온다.</td></tr><tr><td>Cursor Position</td><td>현재 커서의 위치를 나타낸다.</td></tr><tr><td>Fetch Description</td><td>Fetch된  로우의 개수와 시간을 나타낸다.</td></tr></tbody></table>

현재 조회할 수 있는 Tibero Database 데이터 타입은 다음과 같다. 🤷‍♂️~~CLOB, BLOB과 같은 대용량 데이터 타입 혹은 사용자 데이터 타입에 대한 조회는 지원하지 않고 있다.~~

* NUMBER, BINARY\_FLOAT, BINARY\_DOUBLE
* CHAR, VARCHAR, VARCHAR2, RAW
* DATE, TIMESTAMP, TIMESTAMP WITH TIME ZONE, TIMESTAMP WITH LOCAL TIME ZONE
* INTERVAL YEAR TO MONTH, INTERVAL DAY TO SECOND



### **실행 계획**

Editor 영역에 SQL 문장을 입력하고 **SQL Editor 화면**([\[그림 3.6\]](https://technet.tmax.co.kr/upload/download/online/tibero/pver-20230906-000001/user-guide/chapter03.html#figure\_sqleditor\_full)) 상단에 위치한 **\[Plan] 버튼**을 클릭하면 View 영역에 해당 SQL 문장의 실행 계획이 조회된다. 사용자는 이 계획을 통해 자신이 작성한 SQL 문장의 실행 계획을 확인할 수 있다.  또한 상단에 위치한 \[SQL Trace] 버튼을 클릭하여 쿼리를 실제로 수행하고 예측된 Plan과 수행된 Plan을 조회할 수 있다.

&#x20;쿼리 튜닝이 필요하면 이를 수행하여 최적의 SQL 문장을 작성할 수도 있다.

#### Execution Plan

Execution Plan에서는 작성한SQL 정보와  Plan의 Tree/Text View 를 제공한다. 또한 각 Row별 세부정보를 제공한다.&#x20;

<figure><img src="../../../../.gitbook/assets/image (68).png" alt="" width="375"><figcaption><p>[그림 n.3]  Execution Plan</p></figcaption></figure>

#### SQL Trace

SQL Trace에서는 수행된 SQL 정보를 제공하며, SQL 실행 통계정보 및 예측정보에 대해 제공한다. 각 플랜은 모두 Tree/Text View를 제공하며,  각 Row별 세부정보를 제공한다.&#x20;

<figure><img src="../../../../.gitbook/assets/image (71).png" alt="" width="375"><figcaption><p>[그림 n.4] SQL Trace</p></figcaption></figure>

