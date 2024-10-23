---
description: SQL 작성없이 Index를 수정할 수 있는 Operator에 대해 설명한다.
---

# Edit Index GUI Operator

Edit Index User Interface

Schema Tree > Index > Edit 을 선택하면 다음과 같은 창이 열린다.

<figure><img src="../../../../../.gitbook/assets/image (126).png" alt="" width="375"><figcaption><p>Edit Index 창</p></figcaption></figure>

* Edit Index의  각 탭에 대한 자세한 설명은 [Create Index](../create-gui-operator/create-index-gui-operator.md) 와같다

<table><thead><tr><th width="160">항목</th><th>설명</th></tr></thead><tbody><tr><td>Common</td><td>Index의 이름 등 기본적인 정보를  설정한다.</td></tr><tr><td>Columns</td><td>Index를 설정할 컬럼을 선택한다. </td></tr><tr><td>Options</td><td>Index 의 옵션을 설정한다.</td></tr><tr><td>Partitions</td><td>저장영역에 대해 옵션을 설정한다.</td></tr></tbody></table>

### Common

Common 탭에서는 Index의 기본적인 정보를 설정할 수 있으며, Common 탭의 화면과 각 항목에 대한 설명은  [Create Index Common](../create-gui-operator/create-index-gui-operator.md#common) 과같다

<figure><img src="../../../../../.gitbook/assets/image (8).png" alt="" width="375"><figcaption><p>Edit Index Common</p></figcaption></figure>

* Schema와 Index Type은 변경이 불가능하다.

### Columns

Columns 탭에서는Index를 설정할 컬럼을 선택할 수 있다. 각 항목에 대한 자세한 설명은 [Create Index Column](../create-gui-operator/create-index-gui-operator.md#columns) 과 같다.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (9).png" alt="" width="375"><figcaption><p>Edit Index Columns</p></figcaption></figure>

### Options

Options 탭에서는 인덱스의 옵션을 설정한다. 각 항목에 대한 자세한 설명은  [Create Index Column](../create-gui-operator/create-index-gui-operator.md#option) 과 같다.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (11).png" alt="" width="375"><figcaption><p>Edit Index Options</p></figcaption></figure>

### Partitions

Partitions 탭에서는 인덱스 파티셔닝에 대해 상세한 설정을 할 수 있다. 각 항목에 대한 자세한 설명은  [Create Index Column](edit-index-gui-operator.md#partitions) 과 같다.&#x20;



각 항목에 대한 설명은 다음과 같다.

<table><thead><tr><th width="222">항목</th><th>설명</th></tr></thead><tbody><tr><td>Partition</td><td>파티셔닝 타입을 설정한다.</td></tr><tr><td>Last Partition Column</td><td>Column 탭에서 선택한 컬럼 리스트를 보여준다.</td></tr><tr><td>Partition List</td><td>설정한 파티션의 목록을 보여준다.</td></tr><tr><td>Local Index Partition</td><td>파티션 목록 및 Key 압축여부, Storage Setting 등 세부사항을 설정한다.</td></tr></tbody></table>

