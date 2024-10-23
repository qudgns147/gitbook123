---
description: SQL 작성없이 FGA Policy를 생성할 수 있는 Operator에 대해 설명한다.
---

# Create FGA Policy GUI Operator

## User Interface

Schema Tree > Context Menu > Create FGA Policy을 선택하면, 아래와 같이 Job을 생성할 수 있는 창이 열린다.

<figure><img src="../../../../../.gitbook/assets/image (139).png" alt="" width="375"><figcaption><p>Create FGA Policy</p></figcaption></figure>

Create FGA Policy 각 탭에서 테이블 생성시 설정할 수 있는 다양한 옵션이 있으며 자세한 설명은 다음과 같다

* Create FGA Policy Tab List

<table><thead><tr><th width="201">항목</th><th>설명</th></tr></thead><tbody><tr><td>Options</td><td>Policy의 이름 등 기본적인 정보를  설정한다.</td></tr><tr><td>FGA Condition</td><td>감사 조건을 설정한다.</td></tr></tbody></table>

### Options

<figure><img src="../../../../../.gitbook/assets/image (139).png" alt="" width="375"><figcaption><p>Create FGA Policy</p></figcaption></figure>

* 각 항목에 대한 설명은 다음과 같다.

<table><thead><tr><th width="216">항목</th><th>설명</th></tr></thead><tbody><tr><td>FGA Policy Name</td><td>감시 정책 이름을 선택한다.</td></tr><tr><td>Target Object</td><td><p>감시 대상 오브젝트를 선택한다.</p><p>Schema : 감시 오브젝트의 스키마를 선택한다.</p><p>Object Name : 감시 대상 오브젝트를 선택한다.</p><p>Object Type : 테이블 혹은 뷰를 선택한다.</p></td></tr><tr><td>Specify columns</td><td>감시 대상 컬럼을 선택한다.</td></tr><tr><td>Audit Statement Types</td><td>감사를 적용할 SQL 문장 종류를 선택한다.</td></tr><tr><td>Audit Column Option</td><td><p>ANY_COLUM : 일부 컬럼만 참조해도 감시를 기록한다.</p><p>All_COLUMN : 모든 컬럼을 참조할 때만 감시를 기록한다.</p></td></tr><tr><td>Audit Trail</td><td>감시 기록을 남길 위치와 SQL 구문 및 바인드 변수 기록할지 여부를 선택한다.</td></tr><tr><td>Enabled</td><td>해당 정책을 활성화할지 여부를 선택한다.</td></tr></tbody></table>

### Audit Condition

<figure><img src="../../../../../.gitbook/assets/image (140).png" alt="" width="375"><figcaption><p>Audit Policy</p></figcaption></figure>

* 오브젝트 내 감시 대상 데이터의 행 조건을 특정하기 위한 SQL WHERE 절의 조건식을 입력한다.&#x20;
