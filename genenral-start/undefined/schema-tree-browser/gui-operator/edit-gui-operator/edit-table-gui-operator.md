---
description: SQL 작성없이 Table을 수정할 수 있는 Operator에 대해 설명한다.
---

# Edit Table GUI Operator

User Interface

Schema Tree > Context Menu > Edit Table 를 선택하면, 아래와 같이 테이블에 대한 기본 설정을 하는 탭이 열린다.

<figure><img src="../../../../../.gitbook/assets/image (42).png" alt="" width="375"><figcaption><p>Edit Table - Common Tab</p></figcaption></figure>

Edit Table의 각 탭에서 테이블의 수정시 설정도 가능하며 자세한 사항은 [Create Table](../create-gui-operator/create-table-gui-operator.md)에서 확인 가능하다.

### Common

Common 탭에서는 테이블의 스키마, 이름 등 기본적인 정보를 설정할 수 있으며, Common 탭의 화면과 각 항목에 대한 설명은  Common 과 같다.

<figure><img src="../../../../../.gitbook/assets/image (42).png" alt="" width="375"><figcaption><p>Edit Table - Common Tab</p></figcaption></figure>

* Schema와 Type은 변경이 불가능하다.&#x20;

### Columns

Columns 탭에서는 테이블의 컬럼 이름과 데이터 타입, 암호화 등 옵션을 설정할 수 있으며 자세한 설명은 [Create Table](../create-gui-operator/create-table-gui-operator.md#columns)[ Column](edit-table-gui-operator.md) 같다.

<figure><img src="../../../../../.gitbook/assets/image (43).png" alt="" width="375"><figcaption><p>Edit Table - Columns Tab</p></figcaption></figure>

### Constraints

Constraints 탭에서는 테이블의 제약조건을 설정하고 조회할 수 있으며, 각  탭에 대한 설명은 [Create Table Constraint](../create-gui-operator/create-table-gui-operator.md#constraints)과 같다.

<figure><img src="../../../../../.gitbook/assets/image (23).png" alt="" width="375"><figcaption><p>Edit Table - Constraint</p></figcaption></figure>

* Type 변경이 불가능 하다.

### Indexes

Index 탭에서는 테이블의 인덱스를 설정하고 조회할 수 있으며 자세한 설명은 [Create Table Index](../create-gui-operator/create-table-gui-operator.md#indexes)과 같다.

<figure><img src="../../../../../.gitbook/assets/image (25).png" alt="" width="375"><figcaption><p>Edit Table - Index</p></figcaption></figure>

### Storage

Storage Tab에서는 테이블 스페이스, 세그먼트 세부 속성 등을 설정할 수 있다. 자세한 설명은 [Create Table  Storage](../create-gui-operator/create-table-gui-operator.md#storage) 와같다.

<figure><img src="../../../../../.gitbook/assets/image (26).png" alt="" width="375"><figcaption></figcaption></figure>

### Partitions

* Partition Tab에서는 파티션 또는 서브파티션의 타입과 컬럼을 설정할 수 있다. 자세한 설명은 [Create Table Partition](../create-gui-operator/create-table-gui-operator.md#partitions) 같다.

<figure><img src="../../../../../.gitbook/assets/image (27).png" alt="" width="375"><figcaption><p>Edit Table Partition</p></figcaption></figure>

* Partition Detail 에서는 파티션 타입에 적용할 상세 정보를 설정한다. 자세한 설명은 [Tibero Manual](https://technet.tmax.co.kr/upload/download/online/tibero/pver-20240821-000001/sql-reference/ch\_ddl.html#sect\_ddl\_ALTER\_TABLE)을 참조한다.

### Comment

Comment Tab에서는테이블에 대한 코멘트를 남길 수 있다.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (28).png" alt="" width="375"><figcaption><p>Edit Table Comment</p></figcaption></figure>

* Temporary Table  등 다른 테이블  타입에 대한 GUI Operator 또한 지원한다.&#x20;

