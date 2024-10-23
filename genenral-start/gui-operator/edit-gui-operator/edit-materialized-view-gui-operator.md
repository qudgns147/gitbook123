---
description: SQL 작성없이 Materialized View를 수정할 수 있는 Operator에 대해 설명한다.
---

# Edit Materialized View GUI Operator

## User Interface

Schema Tree > Materialized View > Context Menu > Edit 를 선택하면 다음과 같은 Materialized View를 수정하는 창이 열린다.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (33).png" alt="" width="375"><figcaption><p>Edit Materialized View</p></figcaption></figure>

Edit Materialized View의 각 탭에서 테이블 생성시 설정할 수 있는 다양한 옵션이 있으며 자세한 설명은 [Create Materialized View](../create-gui-operator/create-materialized-view-gui-operator.md#user-interface)과 같다

### Common

Common 탭에서는 스키마, 이름 등 기본적인 정보를 설정할 수 있으며, 각 항목에 대한 설명은 [Create Materialized View](../create-gui-operator/create-materialized-view-gui-operator.md#common)과 같다.

<figure><img src="../../../../../.gitbook/assets/image (34).png" alt="" width="375"><figcaption><p>Edit Materialized View  Common</p></figcaption></figure>

### Query

Query 탭은 Materialized View를 생성하기 위해 쿼리를 테스트 하는 탭으로, 사용자가 쿼리를 작성하여 테스트를 수행할 수 있다.

<figure><img src="../../../../../.gitbook/assets/image (35).png" alt="" width="375"><figcaption><p>Edit Materialized View</p></figcaption></figure>

### Materialized View Info

Material View Info 탭에서는 해당 View의 다양한 옵션을 설정한다. 각 항목에 대한 설명은 [Create Materialized View Info ](../create-gui-operator/create-materialized-view-gui-operator.md#materialized-view-info)와 같다

<figure><img src="../../../../../.gitbook/assets/image (55).png" alt="" width="375"><figcaption><p>Materialized View Info</p></figcaption></figure>

### Storage

Storage Tab에서는 테이블 스페이스, 세그먼트 세부 속성 등을 설정할 수 있다. 자세한 설명은 [Create Materialized Storage](../create-gui-operator/create-materialized-view-gui-operator.md#storage) 와같다.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (36).png" alt="" width="375"><figcaption><p>Materialized View Storage</p></figcaption></figure>

### Indexes

Indexes 탭에서는 Materialized View의인덱스를 설정하고 조회할 수 있다.

<figure><img src="../../../../../.gitbook/assets/image (37).png" alt="" width="375"><figcaption><p>Edit Materialized View Index</p></figcaption></figure>

* 왼쪽 리스트는 인덱스의 리스트를 나타내며, +/- 버튼을 통해 인덱스를 추가/삭제할 수 있으며 화살표 버튼을 통해 순서를 변경할 수 있다. 또한 Reset 버튼을 통해 설정한 모든 인덱스를 초기화 할 수 있다.&#x20;
* 오른쪽 상세 설정 창에서는 Index의 상세 정보를 설정할 수 있으며 자세한 사항은 [Create Materialized Indexes](../create-gui-operator/create-materialized-view-gui-operator.md#indexes) 와 같다.

### Partitions

* Partition Tab에서는 파티션 또는 서브파티션의 타입과 컬럼을 설정할 수 있다. 각 항목에 대한 자세한 설명은 [Create Materialized Partitions](../create-gui-operator/create-materialized-view-gui-operator.md#partitions) 와 같다.

<figure><img src="../../../../../.gitbook/assets/image (39).png" alt="" width="375"><figcaption><p>Edit Materialized View Partitions</p></figcaption></figure>

### Comment

Comment Tab에서는 View에 대한 코멘트를 남길 수 있다.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (38).png" alt="" width="375"><figcaption></figcaption></figure>
