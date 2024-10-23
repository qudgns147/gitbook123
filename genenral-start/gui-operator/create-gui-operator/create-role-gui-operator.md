---
description: SQL 작성없이 Role을 생성할 수 있는 Operator에 대해 설명한다.
---

# Create Role GUI Operator

## User Interface

Schema Tree > Context Menu > Create Role 선택하면 다음과 같은 창이 열린다.



<figure><img src="../../../../../.gitbook/assets/image (63).png" alt="" width="375"><figcaption><p>Create Role UI</p></figcaption></figure>

Create Role의 각 탭에서 Role 생성시 설정할 수 있는 다양한 옵션이 있으며 자세한 설명은 다음과 같다

* Create View Tab List

<table><thead><tr><th width="200">항목</th><th>설명</th></tr></thead><tbody><tr><td>Common</td><td>View의 이름 등 기본적인 정보를  설정한다.</td></tr><tr><td>System Privilege</td><td>Role 이 부여받을 시스템 권한을 설정한다.</td></tr><tr><td>Object Privilege</td><td>Role이 부여받을 오브젝트 권한을 설정한다.</td></tr><tr><td>Role</td><td>Role이 부여받을 Role을 설정한다. </td></tr></tbody></table>

### Common

Common 탭에서는 스키마, 이름 등 기본적인 정보를 설정할 수 있으며, Common 탭의 화면과 각 항목에 대한 설명은 다음과 같다.

<figure><img src="../../../../../.gitbook/assets/image (49).png" alt="" width="375"><figcaption><p>Create Role - Common</p></figcaption></figure>

<table><thead><tr><th width="150">항목</th><th>설명</th></tr></thead><tbody><tr><td>Name</td><td>Role의 이름을 설정한다.</td></tr><tr><td>Type</td><td> 패스워드를 사용할지 여부를 설정한다.</td></tr></tbody></table>



### System Privilege

System Privilege 탭에서는 Role에 부여할 시스템 권한을 선택하여 설정할 수 있다.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (50).png" alt="" width="375"><figcaption><p>Privilege tab</p></figcaption></figure>

* 각 항목에 대한 자세한 설명은 다음과 같다.

| 항목               | 설명                          |
| ---------------- | --------------------------- |
| System Privilege | 시스템 권한의 이름을 나타낸다.           |
| Grant            | 시스템 권한을 Role의 부여한다.         |
| Admin            | 시스템 권한을 Grant할 권한도 함께 부여한다. |



### Object Privilege

Object Privilege 탭에서는 Role에 부여할 오브젝트에 대한 권한을 설정할 수 있다.

<figure><img src="../../../../../.gitbook/assets/image (51).png" alt="" width="375"><figcaption><p>Object Privilege</p></figcaption></figure>

* 각 Row를 선택하여 권한을 추가/삭제할 수 있다. 각 항목에 대한  자세한 설명은 다음과 같다.

<table><thead><tr><th width="209">항목</th><th>설명</th></tr></thead><tbody><tr><td>+/-</td><td>Role에 권한을 부여할 오브젝트를 추가/삭제한다.</td></tr><tr><td>Schema</td><td>권한 부여 대상 오브젝트의 소유자를 나타낸다.</td></tr><tr><td>Object Type</td><td>권한 부여 대상 오브젝트의 타입을 나타낸다.</td></tr><tr><td>Object Name</td><td>권한 부여 대상 오브젝트의 이름을 나타낸다.</td></tr><tr><td>Privilege</td><td>부여할 권한을 나타낸다.</td></tr></tbody></table>

### Role

Role 탭에서는 Role에 부여할 Role을 설정한다.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (52).png" alt="" width="375"><figcaption><p>Role Tab</p></figcaption></figure>

* 각 항목에 대한 자세한 설명은 다음과 같다.

<table><thead><tr><th width="209">항목</th><th>설명</th></tr></thead><tbody><tr><td>Role</td><td>Role에 부여할 Role의 이름을 나타낸다.</td></tr><tr><td>Grant</td><td>권한 부여 여부를 나타낸다.</td></tr><tr><td>Default</td><td>Role의 기본권한 활성화 여부를 나타낸다.</td></tr><tr><td>Admin</td><td>해당 Role을 Grant할 권한도 함께 부여한다.</td></tr></tbody></table>
