---
description: SQL 작성없이 Materialized View를 생성할 수 있는 Operator에 대해 설명한다.
---

# Create Materialized View GUI Operator

## User Interface

Schema Tree > Context Menu >  Create >  Materialized View를 선택하면 다음과 같은 Materialized View를 생성하는 창이 열린다.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (53).png" alt="" width="375"><figcaption><p>Create Materized View </p></figcaption></figure>

Create Materialized View의 각 탭에서 테이블 생성시 설정할 수 있는 다양한 옵션이 있으며 자세한 설명은 다음과 같다

* Create Materialized View Tab List

<table><thead><tr><th width="160">항목</th><th>설명</th></tr></thead><tbody><tr><td>Common</td><td>Materialized  View의 이름 등 기본적인 정보를  설정한다.</td></tr><tr><td>Query</td><td>Materialized  View를 생성할 Query 를 작성하고 테스트 한다.</td></tr><tr><td>Materialized View Info</td><td>Materialized View의 옵션을 설정한다.</td></tr><tr><td>Storage</td><td>저장영역에 대해 옵션을 설정한다.</td></tr><tr><td>Index</td><td>Materialized View의 Index를 설정한다. </td></tr><tr><td>Partition</td><td>Partition 여부 및 옵션 등을 설정한다.</td></tr><tr><td>Comment</td><td>코멘트를 작성한다.</td></tr></tbody></table>



### Common

Common 탭에서는 스키마, 이름 등 기본적인 정보를 설정할 수 있으며, Common 탭의 화면과 각 항목에 대한 설명은 다음과 같다.

<figure><img src="../../../../../.gitbook/assets/image (53).png" alt="" width="375"><figcaption><p>Create Materized View </p></figcaption></figure>

<table><thead><tr><th width="150">항목</th><th>설명</th></tr></thead><tbody><tr><td>Schema</td><td>현재 접속정보에서 조회 가능한 스키마를 표시한다.</td></tr><tr><td>Name</td><td>테이블의 이름을 설정한다.</td></tr><tr><td>Type</td><td>생성할 테이블의 타입을 설정한다.</td></tr></tbody></table>

### Query

Query 탭은 View를 생성하기 위해 쿼리를 테스트 하는 탭으로, 사용자가 쿼리를 작성하여 테스트를 수행할 수 있다.

<figure><img src="../../../../../.gitbook/assets/image (54).png" alt="" width="375"><figcaption><p>[그림 n.3] Query Tab</p></figcaption></figure>

* 사용자가 쿼리를 작성하여 테스트를 수행하고, 해당 쿼리를 Materialized View로 생성한다.

### Materialized View Info

View Info 탭에서는 해당 View의 다양한 옵션을 설정한다.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (55).png" alt="" width="375"><figcaption><p>Materialized View Info</p></figcaption></figure>

* 각 항목에 대한 자세한 설명은 다음과 같다.

<table><thead><tr><th width="198">항목</th><th>설명</th></tr></thead><tbody><tr><td>Refresh Mode</td><td><p>Refresh를 언제 수행할지 결정한다.</p><p>On Demand : Refresh 호출 시에 새로고침한다.</p><p>On Commit : 마스터 테이블에 커밋이 일어날 때 마다 새로고침한다.</p><p>Time : 새로고침 할 시간을 설정한다.</p></td></tr><tr><td>Refresh Method</td><td><p>Refresh 방법을 선택한다.</p><p>Force : Fast Refresh가 가능하면 Fast Refresh하고 불가능할 경우 Complete Refresh를 수행한다.</p><p>Fast : Fast Refresh를 수행한다.</p><p>Complete : Query를 재 수행하여 Refresh 한다.</p></td></tr><tr><td>With</td><td>Row ID 혹은 Primary Key를 사용하여 새로고침 한다.</td></tr><tr><td>Build Mode</td><td>데이터를 언제 삽입할 것인지 설정한다.</td></tr><tr><td>Query Rewrite Enable</td><td>Query를 다시쓰기에 사용될 수 있는지(Create table as Select etc.) 여부를 설정한다.</td></tr></tbody></table>

### Storage

Storage Tab에서는 테이블 스페이스, 세그먼트 세부 속성 등을 설정할 수 있다.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (56).png" alt="" width="375"><figcaption><p>Create MView  > Storage Tab</p></figcaption></figure>

* 각 항목에 대한 자세한 설명은 다음과 같다.

<table><thead><tr><th width="278">항목</th><th>설명</th></tr></thead><tbody><tr><td> Compress</td><td> 압축 여부를 설정한다.</td></tr><tr><td>Degree Of Parallelism (DOP)</td><td>병렬 처리를 위한 워킹 스레드의 개수를 설정한다.</td></tr><tr><td>Segment Settings</td><td>물리적 저장 공간을 설정한다.</td></tr><tr><td>Tablespace</td><td>데이터가 저장될 테이블스페이스를 설정한다.</td></tr><tr><td>PCT Free</td><td>데이터 블록의 예비 영역의 크기를 설정한다.</td></tr><tr><td>Initrans</td><td>트랜잭션 엔트리의 초기 값을 설정한다.</td></tr><tr><td>Logging</td><td>Redo Log를 남길지 여부를 선택한다.</td></tr><tr><td>Storage Option</td><td>세그먼트의 세부적인 속성을 선택한다.</td></tr><tr><td>Max Extents</td><td>세그먼트에 할당되는 최대 익스텐트의 개수를 지정한다.</td></tr><tr><td>Buffer Pool</td><td>세그먼트를 어떤 Buffer Pool에 넣을 것인지 선택한다.</td></tr></tbody></table>

### Indexes

Index 탭에서는 Materialized View의인덱스를 설정하고 조회할 수 있다.

<figure><img src="../../../../../.gitbook/assets/image (57).png" alt="" width="375"><figcaption><p>Materialized View > Index Tab</p></figcaption></figure>

* 왼쪽 리스트는 인덱스의 리스트를 나타내며, +/- 버튼을 통해 인덱스를 추가/삭제할 수 있으며 화살표 버튼을 통해 순서를 변경할 수 있다. 또한 Reset 버튼을 통해 설정한 모든 인덱스를 초기화 할 수 있다.&#x20;
* 오른쪽 상세 설정 창에서는 Index의 상세 정보를 설정할 수 있으며 자세한 사항은 다음과 같다.

<table><thead><tr><th width="211">항목</th><th>설명</th></tr></thead><tbody><tr><td>Index Settings</td><td>인덱스의 기본정보를 설정한다.</td></tr><tr><td>Index Type</td><td>Index의 타입을 설정 한다.</td></tr><tr><td>Index Name</td><td>Index의 이름을 설정한다.</td></tr><tr><td>Column Settings</td><td><p>인덱스 컬럼의 정보를 설정한다.</p><p>-      Column : 사용자가 설정한 컬럼 리스트 표시</p><p>-      Expression : 인덱스 키로 설정한 컬럼의 이름 또는 표현식</p><p>-      Order : 컬럼 내 데이터의 정렬 순서</p></td></tr></tbody></table>

### Partitions

* Partition Tab에서는 파티션 또는 서브파티션의 타입과 컬럼을 설정할 수 있다.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (74).png" alt="" width="375"><figcaption><p>[그림n.8] Create Table > Partition Tab</p></figcaption></figure>

* 각 항목에 대한 자세한 설명은 다음과 같다.

<table><thead><tr><th width="200">항목</th><th>설명</th></tr></thead><tbody><tr><td>Partition Type</td><td>파티션의 타입을 설정한다.</td></tr><tr><td>Select Column</td><td>파티션 분리할 기준이 될 파티션키 컬럼을 선택한다.</td></tr></tbody></table>

* Partition Detail 에서는 파티션 타입에 적용할 상세 정보를 설정한다. 자세한 설명은 다음과 같다.

<figure><img src="../../../../../.gitbook/assets/image (75).png" alt="" width="375"><figcaption><p>[그림n.9] Create Table > Partition Tab > Partition Detail</p></figcaption></figure>

* 오른쪽에서 파티션 별 상세한 설정을 할 수 있으며 자세한 설명은 다음과 같다.

<table><thead><tr><th width="228">항목</th><th>설명</th></tr></thead><tbody><tr><td>Partition Type / Sub Partition Type</td><td>Partition Type 설정 화면에서 설정한 파티션/서브파티션 타입을 표시한다.</td></tr><tr><td>Change Partition Type</td><td>설정하던 정보를 초기화하고 Partition Type 설정 창으로 돌아간다.</td></tr><tr><td>Partition Name</td><td>파티션의 이름을 설정한다.</td></tr><tr><td>Partition Detail</td><td>각 파티션 별 Value의 기준을 설정한다.</td></tr><tr><td>Table Compression &#x26; Storage Settings</td><td><a href="create-materialized-view-gui-operator.md#storage">Storage Tab 참조</a></td></tr></tbody></table>

### Comment

Comment Tab에서는 View에 대한 코멘트를 남길 수 있다.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (59).png" alt="" width="375"><figcaption><p>Materialized View > Comment</p></figcaption></figure>
