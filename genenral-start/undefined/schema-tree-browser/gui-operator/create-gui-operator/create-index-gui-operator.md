---
description: SQL 작성없이 Index를 생성할 수 있는 Operator에 대해 설명한다.
---

# Create Index GUI Operator

## Create Index User Interface

Schema Tree > Context Menu > Create Index를 선택하면 다음과 같은 창이 열린다.

<figure><img src="../../../../../.gitbook/assets/image (126).png" alt="" width="375"><figcaption><p>[그림] Create Index 창</p></figcaption></figure>

* Create Index 의 각 탭에자대한세한 설명은 다음과 같다

<table><thead><tr><th width="160">항목</th><th>설명</th></tr></thead><tbody><tr><td>Common</td><td>Index의 이름 등 기본적인 정보를  설정한다.</td></tr><tr><td>Columns</td><td>Index를 설정할 컬럼을 선택한다. </td></tr><tr><td>Options</td><td>Index 의 옵션을 설정한다.</td></tr><tr><td>Partitions</td><td>저장영역에 대해 옵션을 설정한다.</td></tr></tbody></table>

### Common

Common 탭에서는 Index의 기본적인 정보를 설정할 수 있으며, Common 탭의 화면과 각 항목에 대한 설명은 다음과 같다.

<figure><img src="../../../../../.gitbook/assets/image (126).png" alt="" width="375"><figcaption><p>[그림] Create Index 창</p></figcaption></figure>

<table><thead><tr><th width="150">항목</th><th>설명</th></tr></thead><tbody><tr><td>Schema</td><td>생성될 Object를 소유할 스키마를 선택한다.</td></tr><tr><td>Name</td><td>인덱스의 이름을 설정한다.</td></tr><tr><td>Index Type</td><td>생성할 인덱스의 타입을 설정한다. 인덱스 타입에 따라 주요 설정 정보가 달라 진다. </td></tr></tbody></table>



### Columns

Columns 탭에서는Index를 설정할 컬럼을 선택할 수 있다.

<figure><img src="../../../../../.gitbook/assets/image (128).png" alt="" width="375"><figcaption><p>Create Index Columns</p></figcaption></figure>

* 각 항목에 대한 설명은 다음과 같다.&#x20;

<table><thead><tr><th width="162">항목</th><th>설명</th></tr></thead><tbody><tr><td>No.</td><td>인덱스로 설정할 컬럼의 순서를 나타낸다.</td></tr><tr><td>Schema</td><td>대상이 될 오브젝트의 소유자를 선택한다.</td></tr><tr><td>Table</td><td>대상이 될 테이블을 선택한다.</td></tr><tr><td>Select Column</td><td><p>해당 테이블 내 인덱스로 설정할 컬럼을 선택한다.</p><ul><li>Column : 대상이 될 컬럼을 선택한다.</li><li>Expression : 컬럼의 이름 또는 표현식을 나타낸다.</li><li>Order : 컬럼 값의 정렬 순서를 선택한다.</li><li>Prefix Length : 해당 컬럼의 해당 값 만큼 인덱스로 저장한다.</li></ul></td></tr></tbody></table>

### Option

Option 탭에서는 인덱스의 옵션을 설정한다.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (129).png" alt="" width="375"><figcaption><p>Index Option tab</p></figcaption></figure>

* 각 항목에 대한 자세한 설명은 다음과 같다.

<table><thead><tr><th width="210">항목</th><th>설명</th></tr></thead><tbody><tr><td>Key Compression</td><td>Key를 압축할지 여부를 선택한다.</td></tr><tr><td>DOP (Degree of Parallel)</td><td>병렬 처리를 위한 워킹 스레드의 개수를 설정한다.</td></tr><tr><td>Invisible</td><td>Optimizer가 인덱스를 사용하게 할지 여부를 선택한다.</td></tr><tr><td>Options</td><td><p>다양한 옵션을 설정한다.</p><p>Reverse : 인덱스 블록의 순서를 역으로 저장한다.</p><p>Online : 인덱스 생성 중 DML 허용여부를 선택한다.</p><p>Compute Statistics : 인덱스 통계정보를 수집한다.  </p></td></tr><tr><td>TDE-Range Scan</td><td>암호화 테이블의 인덱스를 이용하여 Range Scan 할지 여부를 선택한다.</td></tr><tr><td>Storage Settings</td><td><p>저장 공간에 대해 설정한다.</p><p>PCT Free : 데이터 블록의 예비 영역의 크기를 설정한다.</p><p>Initrans : 트랜잭션 엔트리의 초기 값을 설정한다.</p><p>Tablespace : 데이터가 저장될 테이블스페이스를 설정한다.</p><p>Max Extents : 세그먼트에 할당되는 최대 익스텐트의 개수를 지정한다.</p><p>Buffer Pool : 세그먼트를 어떤 Buffer Pool에 넣을 것인지 선택한다.</p></td></tr></tbody></table>

### Partitions

Partitions 탭에서는 인덱스 파티셔닝에 대해 상세한 설정을 할 수 있다.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (130).png" alt="" width="375"><figcaption><p>그림 인덱스 파티셔닝</p></figcaption></figure>

* 각 항목에 대한 설명은 다음과 같다.

<table><thead><tr><th width="222">항목</th><th>설명</th></tr></thead><tbody><tr><td>Partition</td><td>파티셔닝 타입을 설정한다.</td></tr><tr><td>Last Partition Column</td><td>Column 탭에서 선택한 컬럼 리스트를 보여준다.</td></tr><tr><td>Partition List</td><td>설정한 파티션의 목록을 보여준다.</td></tr><tr><td>Local Index Partition</td><td>파티션 목록 및 Key 압축여부, Storage Setting 등 세부사항을 설정한다.</td></tr></tbody></table>

