---
description: SQL 작성없이 Sequence 를 생성할 수 있는 Operator에 대해 설명한다.
---

# Create Sequence GUI Operator

## Create Sequnced UI

Create Sequence를 선택하면 다음과 같은 창이 열린다.

<figure><img src="../../../../../.gitbook/assets/image (61).png" alt="" width="375"><figcaption><p>Create Sequence</p></figcaption></figure>

* 각 항목에 대한 설명은 다음과 같다.

<table><thead><tr><th width="164">항목</th><th>설명</th></tr></thead><tbody><tr><td>Schema</td><td>Sequence 소유자를 선택한다.</td></tr><tr><td>Name</td><td>Sequence의 이름을 입력한다.</td></tr><tr><td>Start With</td><td>Sequence의 시작 값을 지정한다.</td></tr><tr><td>Increment</td><td>Sequence의 간격을 지정한다. 음수일 경우 Sequence 값이 감소한다.</td></tr><tr><td>Min Value</td><td>Sequence의 최소값을 설정한다.</td></tr><tr><td>Max Value</td><td>Sequence의 최대값을 설정한다.</td></tr><tr><td>Cache</td><td>Cache에 Cache Size 만큼 저장할지 여부를 결정한다.</td></tr><tr><td>Cycle</td><td>값을 계속해서 생성할지 여부를 설정한다.</td></tr><tr><td>Order</td><td>클러스터 환경에서 노드간 Sequence 순서를 유지할지 설정한다.</td></tr></tbody></table>
