---
description: >-
  본 장에서는 사용자가 주로 사용하는 Schema Tree Browser와 View 영역의 SQL Editor, PSM Editor,
  Schema Object Detail 화면 구성과 사용 방법을 설명한다.
---

# Schema Tree Browser

## Schema Tree Browser <a href="#d5e1845" id="d5e1845"></a>

Tibero Studio의 초기 화면의 왼쪽에 위치하는 **Schema Tree Browser 화면**에서 Tibero Studio과 연결을 유지하고 있는 데이터베이스의 스키마 객체의 정보를 트리 형태로 조회할 수 있다. 해당 화면이 보이지 않으면 **\[View] > \[Schema Tree Browser]** 메뉴를 선택한다.

다음은 Schema Tree Browser 화면의 세부 기능에 대한 설명이다.

<figure><img src="../../../.gitbook/assets/image (94).png" alt="" width="375"><figcaption><p>[그림 3.1] Schema Tree Browser 화면</p></figcaption></figure>

## **Object List**

Schema Tree Browser에서 확인할 수 있는 Object List는 다음과 같다.

<table><thead><tr><th width="199">구분</th><th>설명</th></tr></thead><tbody><tr><td>유저 오브젝트</td><td><ul><li>Table</li><li>View</li><li>Index</li><li>Trigger</li><li>Package</li><li>Procedure</li><li>Function </li><li>Type</li><li>Sequence</li><li>Materialized View</li><li>Materialized View Log</li><li>Synonym</li><li>DB Link</li><li>Library</li><li>Job</li><li>Scheduler</li><li>AQ</li><li>JAVA</li><li>FGA Policy</li><li>Tablespace</li><li>Directory</li><li>Security</li></ul></td></tr></tbody></table>

*   **컨텍스트 메뉴**

    **Schema Tree Browser 화면** 상단 영역에서 스키마 객체를 선택한 뒤 오른쪽 마우스 버튼을 클릭하면 컨텍스트 메뉴가 나타난다. 단, 컨텍스트 메뉴는 각 스키마 객체마다 다르게 나타난다.

    컨텍스트 메뉴를 사용하면 스키마 객체를 생성하고, 수정, 삭제할 수 있다. 스키마 객체를 생성, 수정, 삭제하는 것은 별도의 SQL 문장을 작성할 필요 없이 해당 화면에 항목을 채우는 방식으로 진행된다.

<figure><img src="../../../.gitbook/assets/image (97).png" alt="" width="375"><figcaption><p>[그림 3.1] Schema Tree Browser Context Menu</p></figcaption></figure>

<table><thead><tr><th width="323">메뉴</th><th>설명</th></tr></thead><tbody><tr><td><strong>[New Script]</strong></td><td>새로운 SQL Editor를 연다.</td></tr><tr><td><strong>[New Connect]</strong></td><td>새롭게 데이터베이스에 연결을 맺는다.</td></tr><tr><td><strong>[Show Connected Only]</strong></td><td>현재 연결된 접속정보만 보도록 한다.</td></tr><tr><td><strong>[Collapse Node]</strong></td><td>펼쳐져 있는 모든 하위항목을 접는다.</td></tr><tr><td><strong>[Refresh]</strong></td><td>[모든 정보를 새로고침한다.</td></tr></tbody></table>
