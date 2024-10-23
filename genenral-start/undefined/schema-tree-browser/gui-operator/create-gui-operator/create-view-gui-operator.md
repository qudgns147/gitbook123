---
description: SQL 작성없이 View를 생성할 수 있는 Operator에 대해 설명한다.
---

# Create View GUI Operator

## User Interface

Schema Tree에서 Context Menu를 통해 Create View 를 선택하면 다음과 같은 View를 생성하는 창이 열린다.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (119).png" alt="" width="375"><figcaption><p>[그림 n.1] Create View UI</p></figcaption></figure>

Create View의 각 탭에서 테이블 생성시 설정할 수 있는 다양한 옵션이 있으며 자세한 설명은 다음과 같다

* Create View Tab List

<table><thead><tr><th width="200">항목</th><th>설명</th></tr></thead><tbody><tr><td>Common</td><td>View의 이름 등 기본적인 정보를  설정한다.</td></tr><tr><td>Query</td><td>View를 생성할 Query 를 작성하고 테스트 한다.</td></tr><tr><td>View Info</td><td>View의 옵션을 설정한다.</td></tr><tr><td>Comment</td><td>코멘트를 작성한다.</td></tr></tbody></table>



### Common

ommon 탭에서는 테이블의 스키마, 이름 등 기본적인 정보를 설정할 수 있으며, Common 탭의 화면과 각 항목에 대한 설명은 다음과 같다.

<figure><img src="../../../../../.gitbook/assets/image (83).png" alt="" width="375"><figcaption><p>[그림n.2] Create View > Common Tab</p></figcaption></figure>

<table><thead><tr><th width="150">항목</th><th>설명</th></tr></thead><tbody><tr><td>Schema</td><td>현재 접속정보에서 조회 가능한 스키마를 표시한다.</td></tr><tr><td>Name</td><td>테이블의 이름을 설정한다.</td></tr><tr><td>Type</td><td>생성할 테이블의 타입을 설정한다.</td></tr></tbody></table>

### Query

Query 탭은 View를 생성하기 위해 쿼리를 테스트 하는 탭으로, 사용자가 쿼리를 작성하여 테스트를 수행할 수 있다.

&#x20;

<figure><img src="../../../../../.gitbook/assets/image (122).png" alt="" width="375"><figcaption><p>[그림 n.3] Query Tab</p></figcaption></figure>

* 사용자가 쿼리를 작성하여 테스트를 수행하고, 해당 쿼리를 View로 생성한다.

### View Info

View Info 탭에서는 해당 View의 다양한 옵션을 설정한다.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (123).png" alt="" width="375"><figcaption><p>[그림 n.4] View Info Tab</p></figcaption></figure>

* 각 항목에 대한 자세한 설명은 다음과 같다.

<table><thead><tr><th width="153">항목</th><th>설명</th></tr></thead><tbody><tr><td>Force</td><td>Object의 존재 및 권한과 관계 없이 View를 생성한다.</td></tr><tr><td>Restriction</td><td><p>Subquery에 대한 속성을 정의한다.</p><ul><li>No Restriction : 제한사항 없음</li><li>With Read Only : 읽기 전용, Update 불가</li><li>With Check Option : Select가 가능할 때 Update 허용</li></ul></td></tr></tbody></table>



### Comment

Comment Tab에서는 View에 대한 코멘트를 남길 수 있다.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (124).png" alt="" width="375"><figcaption><p>[그림 n.5] Commnet Tab</p></figcaption></figure>
