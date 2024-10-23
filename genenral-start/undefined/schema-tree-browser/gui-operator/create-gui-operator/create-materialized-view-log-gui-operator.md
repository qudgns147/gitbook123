---
description: SQL 작성없이 Materialized View Log를 생성할 수 있는 Operator에 대해 설명한다.
---

# Create Materialized View Log GUI Operator

## User Interface

Schema Tree > Context Menu >  Create >  Materialized View Log를 선택하면 다음과 같은 Materialized View Log를 생성하는 창이 열린다.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (53).png" alt="" width="375"><figcaption><p>Create Materized View Log </p></figcaption></figure>

Create Materialized View Log의 각 탭에서 테이블 생성시 설정할 수 있는 다양한 옵션이 있으며 자세한 설명은 다음과 같다

* Create Materialized View Log Tab List

<table><thead><tr><th width="200">항목</th><th>설명</th></tr></thead><tbody><tr><td>Common</td><td>Materialized  View Log의 이름 등 기본적인 정보를  설정한다.</td></tr><tr><td>Columns</td><td>Materialized  View를 생성할 Query 를 작성하고 테스트 한다.</td></tr><tr><td>Storage</td><td>저장영역에 대해 옵션을 설정한다.</td></tr></tbody></table>

### Common

Common 탭에서는 스키마, 이름 등 기본적인 정보를 설정할 수 있으며, Common 탭의 화면과 각 항목에 대한 설명은 다음과 같다.

<figure><img src="../../../../../.gitbook/assets/image (53).png" alt="" width="375"><figcaption><p>Create Materized View Log</p></figcaption></figure>

<table><thead><tr><th width="150">항목</th><th>설명</th></tr></thead><tbody><tr><td>Schema</td><td>현재 접속정보에서 조회 가능한 스키마를 표시한다.</td></tr><tr><td>Name</td><td>MView Log의 이름을 설정한다.</td></tr></tbody></table>

### Columns&#x20;

Materialized View Log 에 기록할 컬럼을 설정한다.

<figure><img src="../../../../../.gitbook/assets/image (60).png" alt="" width="375"><figcaption><p>Columns Tab</p></figcaption></figure>

| 항목            | 설명                                          |
| ------------- | ------------------------------------------- |
| New Values    | Materialized View Log에 변경 전/후값 기록 여부를 설정한다. |
| Row ID        | 마스터 테이블의 변경된 Row ID를 기록할지 여부를 설정한다.         |
| Primary Key   | 마스터 테이블의 변경된 Primary Key를 기록할지 여부를 선택한다.    |
| Sequence      | 마스터 테이블의 변경된 순서를 기록할지 여부를 선택한다.             |
| Select Column | Materialized View Log에 기록할 컬럼을 선택한다.        |

### Storage

Storage Tab에서는 테이블 스페이스, 세그먼트 세부 속성 등을 설정할 수 있다. 자세한 설명은 아래와 같다.

<figure><img src="../../../../../.gitbook/assets/image (131).png" alt="" width="375"><figcaption><p>그림 Storage</p></figcaption></figure>

<table><thead><tr><th width="278">항목</th><th>설명</th></tr></thead><tbody><tr><td>Table Compress</td><td>테이블의 압축 여부를 설정한다.</td></tr><tr><td>Degree Of Parallelism (DOP)</td><td>병렬 처리를 위한 워킹 스레드의 개수를 설정한다.</td></tr><tr><td>Segment Settings</td><td>물리적 저장 공간을 설정한다.</td></tr><tr><td>Tablespace</td><td>데이터가 저장될 테이블스페이스를 설정한다.</td></tr><tr><td>PCT Free</td><td>데이터 블록의 예비 영역의 크기를 설정한다.</td></tr><tr><td>Initrans</td><td>트랜잭션 엔트리의 초기 값을 설정한다.</td></tr><tr><td>Logging</td><td>Redo Log를 남길지 여부를 선택한다.</td></tr><tr><td>Storage Option</td><td>세그먼트의 세부적인 속성을 선택한다.</td></tr><tr><td>Max Extents</td><td>세그먼트에 할당되는 최대 익스텐트의 개수를 지정한다.</td></tr><tr><td>Buffer Pool</td><td>세그먼트를 어떤 Buffer Pool에 넣을 것인지 선택한다.</td></tr></tbody></table>
