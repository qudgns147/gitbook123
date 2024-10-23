---
description: GNB > View > Task List, Result > Loading 중 Task List 선택 시
---

# Task List

## Task List <a href="#sect_dbs_connect" id="sect_dbs_connect"></a>

GNB > View > Task List 선택하거나,  Result > Loading 중 \[Task List] 선택 시 Task List 화면이 나타난다.&#x20;

Task List 화면의 UI는 다음과 같다.

<figure><img src="../../../.gitbook/assets/image (142).png" alt="" width="375"><figcaption><p>Task List 화면</p></figcaption></figure>

Task는 실행의 단위를 의미하며, SQL을 실행하거나 PSM 을 컴파일/디버그/실행 했을 때 Task가 생성된다.&#x20;

SQL을 실행했을 경우 Task List 영역에 실행중인 혹은 실행 대기중인 Task 목록이 나타나고, (Delete) 아이콘을 클릭하면 실행 중인 Task 가 종료되고 리스트는 삭제된다.  해당 Task가  실행 중일 경우 다음 Task실행으로 넘어간다.

Task List의 항목은 다음과 같다.

<table><thead><tr><th width="179">항목</th><th>설명</th></tr></thead><tbody><tr><td>Task Run Time</td><td>Task 수행 시작 요청 시간을 나타낸다.</td></tr><tr><td>Query Count</td><td>해당 Task에 포함된 쿼리의 개수</td></tr><tr><td>Task</td><td><p>수행 방식을 나타내다.</p><p>- Run, Run Script, Run All From Cursor, Run New Tab, PSM Compile, PSM Debug, PSM Run</p></td></tr><tr><td>Status</td><td><p>현재 상태를 나타낸다.</p><p>- Pending : 대기중</p><p>- Running : Task 수행 중</p><p>- Complete : 수행완료</p></td></tr></tbody></table>

각 Task row를 클릭하면 Task에서 실행될 SQL들을 확인할 수 있고, 상세한 쿼리는 Task List 하단 쿼리 에서 확인할 수 있다.&#x20;

&#x20;더블 클릭을 통해 해당 쿼리의 결과 창을 확인할 수 있다. 삭제된 Result 탭은 확인할 수 없다.

