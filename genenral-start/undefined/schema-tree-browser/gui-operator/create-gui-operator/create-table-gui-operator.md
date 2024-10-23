---
description: SQL 작성없이 Table을 생성할 수 있는 Operator에 대해 설명한다.
---

# Create Table GUI Operator

## User Interface

Schema Tree > Context Menu > Create Table 를 선택하면, 아래와 같이 테이블에 대한 기본 설정을 하는 탭이 열린다.

<figure><img src="../../../../../.gitbook/assets/image (83).png" alt="" width="375"><figcaption><p>[그림n.1] Create Table GUI Operator</p></figcaption></figure>



Create Table의 각 탭에서 테이블 생성시 설정할 수 있는 다양한 옵션이 있으며 자세한 설명은 다음과 같다

* Create Table Tab List

<table><thead><tr><th width="158">Tab</th><th>설명</th></tr></thead><tbody><tr><td>Common</td><td>Schema, Name 등 기본적인 정보를 설정한다.</td></tr><tr><td>Columns</td><td>생성할 테이블의 컬럼 값을 설정한다.</td></tr><tr><td>Constraints</td><td>테이블의 제약조건을 설정한다.</td></tr><tr><td>Indexes</td><td>테이블의 인덱스를 설정한다.</td></tr><tr><td><del>Encryption</del></td><td><del>테이블의 암호화 여부 및 알고리즘 등을 설정한다.</del></td></tr><tr><td>Storage</td><td>저장 영역을 설정한다.</td></tr><tr><td>Partition</td><td>Partition 여부 및 옵션 등을 설정한다.</td></tr><tr><td>Comment</td><td>코멘트를 작성한다.</td></tr></tbody></table>

### Common

Common 탭에서는 테이블의 스키마, 이름 등 기본적인 정보를 설정할 수 있으며, Common 탭의 화면과 각 항목에 대한 설명은 다음과 같다.

<figure><img src="../../../../../.gitbook/assets/image (83).png" alt="" width="375"><figcaption><p>[그림n.2] Create Table > Common Tab</p></figcaption></figure>

<table><thead><tr><th width="150">항목</th><th>설명</th></tr></thead><tbody><tr><td>Schema</td><td>현재 접속정보에서 조회 가능한 스키마를 표시한다.</td></tr><tr><td>Name</td><td>테이블의 이름을 설정한다.</td></tr><tr><td>Type</td><td>생성할 테이블의 타입을 설정한다.</td></tr></tbody></table>

### Columns

Columns 탭에서는 테이블의 컬럼 이름과 데이터 타입, 암호화 등 옵션을 설정할 수 있으며 자세한 설명은 다음과 같다.

<figure><img src="../../../../../.gitbook/assets/image (77).png" alt="" width="375"><figcaption><p>[그림n.3] Create Table > Columns Tab</p></figcaption></figure>

* 왼쪽 리스트트는  컬럼의 리스트 목록을 나타내며 그 순서를 나타내고 있다. 표시정보는 다음과 같다.

<table><thead><tr><th width="192">항목</th><th>설명</th></tr></thead><tbody><tr><td>+/- </td><td>+/- 버튼을 통해 생성할Column을 추가/삭제할 수 있다.</td></tr><tr><td>PK</td><td>Primary Key 여부를 나타낸다.</td></tr><tr><td>Name</td><td>Column의 이름을 나타낸다.</td></tr><tr><td>Data Type / Size</td><td>각 Column의 데이터 타입과 데이터 사이즈를 나타낸다.</td></tr></tbody></table>

* 오른쪽 항목은 컬럼의 상세 설정정보를 나타내며 자세한 설명은 다음과 같다.

<table><thead><tr><th width="205">항목</th><th>설명</th></tr></thead><tbody><tr><td>Column Name</td><td>Column의 이름을 나타낸다.</td></tr><tr><td>Data Type</td><td>Column의 데이터 타입을 나타낸다.</td></tr><tr><td>Lob Parameter</td><td>Data Type이 LOB 타입일 경우 관련 Parameter를 설정 할 수 있다.</td></tr><tr><td>Size </td><td>선택한 데이터 타입의 데이터 사이즈를 나타낸다.</td></tr><tr><td>Scale? <br>Byte / Char?</td><td>NUMBER/ INTERVAL DAY TO SECOND 타입일 경우 데이터의 크기를 나타낸다.</td></tr><tr><td>Not Null</td><td>Null 허용 여부를 나타낸다.</td></tr><tr><td>Default</td><td>Column의 기본값을 설정한다.</td></tr><tr><td>Encryption</td><td>해당  컬럼을  암호화  한다.</td></tr><tr><td>Encryption Algorithm</td><td>암호화 알고리즘을 선택한다.</td></tr><tr><td>No Salt</td><td>Salt 사용여부를 선택한다.</td></tr><tr><td>Comment</td><td>Column의 코멘트를 설정한다.</td></tr><tr><td>Reset</td><td>모든 Column의 설정 정보를 초기화 한다.</td></tr></tbody></table>

### Constraints

Constraints 탭에서는 테이블의 제약조건을 설정하고 조회할 수 있으며, 자세한 설명은 다음과 같다.

<figure><img src="../../../../../.gitbook/assets/image (44).png" alt="" width="375"><figcaption><p>Edit Table - Constraint</p></figcaption></figure>

* 왼쪽 리스트는 제약조건의 리스트를 나타내며, +/- 버튼을 통해 제약조건을 추가/삭제할 수 있다. 또한 Reset 버튼( )을 통해 설정한 모든 제약조건을 초기화 할 수 있다.&#x20;
* 오른쪽 상세 제약조건을 설정할 수 있으며 Constraint Type 별 자세한 설명은 다음과 같다.
* Primary / Unique Key&#x20;

<table><thead><tr><th width="286">항목</th><th>설명</th></tr></thead><tbody><tr><td>Constraint Info</td><td>제약조건의 기본정보를 설정한다.</td></tr><tr><td>Constraint Type</td><td>제약조건의 타입을 설정한다.</td></tr><tr><td>Constraint Name</td><td>제약조건의 이름을 설정한다.</td></tr><tr><td>Enable</td><td>새로 삽입될 데이터에 제약조건을 적용한다.</td></tr><tr><td>Validate</td><td>이미 테이블에 삽입된 데이터가 제약조건을 만족하는지 체크하고 보장한다.</td></tr><tr><td>Primary/Unique Key Setting</td><td>Primary/Unique Key의 세부 사항을 설정한다.</td></tr><tr><td>Select Column</td><td>Primary / Unique Key로 설정할 컬럼을 선택한다.</td></tr><tr><td>Deferrable State</td><td>제약조건의 검증 시점을 선택할 수 있다.</td></tr></tbody></table>

* Foreign Key

<table><thead><tr><th width="251">항목</th><th>설명</th></tr></thead><tbody><tr><td>Constraint Info</td><td>제약조건의 기본정보를 설정한다.</td></tr><tr><td>Constraint Type</td><td>제약조건의 타입을 설정한다.</td></tr><tr><td>Constraint Name</td><td>제약조건의 이름을 설정한다.</td></tr><tr><td>Enable</td><td>새로 삽입될 데이터에 제약조건을 적용한다.</td></tr><tr><td>Validate</td><td>이미 테이블에 삽입된 데이터가 제약조건을 만족하는지 체크한다.</td></tr><tr><td>Constraint Column</td><td>제약조건을 설정할 컬럼을 선택한다.</td></tr><tr><td>Referenced Column Info</td><td>참조할 컬럼 정보를 설정한다.</td></tr><tr><td>Owner</td><td>참조할 테이블을 소유한 스키마를 선택한다.</td></tr><tr><td>Table</td><td>참조할 테이블을 선택한다.</td></tr><tr><td>Column</td><td>참조할 컬럼을 선택한다.</td></tr><tr><td>On Delete</td><td>참조된 컬럼 값이 삭제될 때 참조하는 컬럼 값에 대한 동작을 설정한다.</td></tr></tbody></table>

* Check

<table><thead><tr><th width="254">항목</th><th>설명</th></tr></thead><tbody><tr><td>Constraint Info</td><td>제약조건의 기본정보를 설정한다.</td></tr><tr><td>Constraint Type</td><td>제약조건의 타입을 설정한다.</td></tr><tr><td>Constraint Name</td><td>제약조건의 이름을 설정한다.</td></tr><tr><td>Enable</td><td>새로 삽입될 데이터에 제약조건을 적용한다.</td></tr><tr><td>Validate</td><td>이미 테이블에 삽입된 데이터가 제약조건을 만족하는지 체크하고 보장한다.</td></tr><tr><td>Check Setting</td><td>체크 제약조건의 세부사항을 설정한다.</td></tr><tr><td>Check Condition</td><td>해당 컬럼의 적용할 조건을 입력한다.</td></tr><tr><td>Deferrable State</td><td>제약조건의 검증 시점을 선택할 수 있다.</td></tr></tbody></table>

### Indexes

Index 탭에서는 테이블의 인덱스를 설정하고 조회할 수 있으며 자세한 설명은 다음과 같다.

<figure><img src="../../../../../.gitbook/assets/image (98).png" alt="" width="375"><figcaption><p>[그림n.5] Create Table > Indexes Tab</p></figcaption></figure>

* 왼쪽 리스트는 인덱스의 리스트를 나타내며, +/- 버튼을 통해 인덱스를 추가/삭제할 수 있으며 화살표 버튼을 통해 순서를 변경할 수 있다. 또한 Reset 버튼을 통해 설정한 모든 인덱스를 초기화 할 수 있다.&#x20;
* 오른쪽 상세 설정 창에서는 Index의 상세 정보를 설정할 수 있으며 자세한 사항은 다음과 같다.

<table><thead><tr><th width="211">항목</th><th>설명</th></tr></thead><tbody><tr><td>Index Settings</td><td>인덱스의 기본정보를 설정한다.</td></tr><tr><td>Index Type</td><td>Index의 타입을 설정 한다.</td></tr><tr><td>Index Name</td><td>Index의 이름을 설정한다.</td></tr><tr><td>Column Settings</td><td><p>인덱스 컬럼의 정보를 설정한다.</p><p>-      Column : 사용자가 설정한 컬럼 리스트 표시</p><p>-      Expression : 인덱스 키로 설정한 컬럼의 이름 또는 표현식</p><p>-      Order : 컬럼 내 데이터의 정렬 순서</p></td></tr></tbody></table>

### Storage

Storage Tab에서는 테이블 스페이스, 세그먼트 세부 속성 등을 설정할 수 있다. 자세한 설명은 아래와 같다.

<figure><img src="../../../../../.gitbook/assets/image (73).png" alt="" width="375"><figcaption><p>[그림n.7] Create Table > Storage Tab</p></figcaption></figure>

<table><thead><tr><th width="278">항목</th><th>설명</th></tr></thead><tbody><tr><td>Table Compress</td><td>테이블의 압축 여부를 설정한다.</td></tr><tr><td>Degree Of Parallelism (DOP)</td><td>병렬 처리를 위한 워킹 스레드의 개수를 설정한다.</td></tr><tr><td>Segment Settings</td><td>물리적 저장 공간을 설정한다.</td></tr><tr><td>Tablespace</td><td>데이터가 저장될 테이블스페이스를 설정한다.</td></tr><tr><td>PCT Free</td><td>데이터 블록의 예비 영역의 크기를 설정한다.</td></tr><tr><td>Initrans</td><td>트랜잭션 엔트리의 초기 값을 설정한다.</td></tr><tr><td>Logging</td><td>Redo Log를 남길지 여부를 선택한다.</td></tr><tr><td>Storage Option</td><td>세그먼트의 세부적인 속성을 선택한다.</td></tr><tr><td>Max Extents</td><td>세그먼트에 할당되는 최대 익스텐트의 개수를 지정한다.</td></tr><tr><td>Buffer Pool</td><td>세그먼트를 어떤 Buffer Pool에 넣을 것인지 선택한다.</td></tr></tbody></table>

### Partitions

* Partition Tab에서는 파티션 또는 서브파티션의 타입과 컬럼을 설정할 수 있다. 자세한 설명은 다음과 같다.

<figure><img src="../../../../../.gitbook/assets/image (74).png" alt="" width="375"><figcaption><p>[그림n.8] Create Table > Partition Tab</p></figcaption></figure>

<table><thead><tr><th width="200">항목</th><th>설명</th></tr></thead><tbody><tr><td>Partition Type</td><td>파티션의 타입을 설정한다.</td></tr><tr><td>Select Column</td><td>파티션 분리할 기준이 될 파티션키 컬럼을 선택한다.</td></tr></tbody></table>

* Partition Detail 에서는 파티션 타입에 적용할 상세 정보를 설정한다. 자세한 설명은 다음과 같다.

<figure><img src="../../../../../.gitbook/assets/image (75).png" alt="" width="375"><figcaption><p>[그림n.9] Create Table > Partition Tab > Partition Detail</p></figcaption></figure>

* 오른쪽에서 파티션 별 상세한 설정을 할 수 있으며 자세한 설명은 다음과 같다.

<table><thead><tr><th width="228">항목</th><th>설명</th></tr></thead><tbody><tr><td>Partition Type / Sub Partition Type</td><td>Partition Type 설정 화면에서 설정한 파티션/서브파티션 타입을 표시한다.</td></tr><tr><td>Change Partition Type</td><td>설정하던 정보를 초기화하고 Partition Type 설정 창으로 돌아간다.</td></tr><tr><td>Partition Name</td><td>파티션의 이름을 설정한다.</td></tr><tr><td>Partition Detail</td><td>각 파티션 별 Value의 기준을 설정한다.</td></tr><tr><td>Table Compression &#x26; Storage Settings</td><td><a href="create-table-gui-operator.md#storage">Storage Tab 참조</a></td></tr></tbody></table>



### Comment

Comment Tab에서는테이블에 대한 코멘트를 남길 수 있다.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (76).png" alt="" width="375"><figcaption><p>[그림n.10] Create Table > Comment Tab</p></figcaption></figure>

Temporary Table  등 다른 테이블에 대한 GUI Operator 또한 지원한다.&#x20;

