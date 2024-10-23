---
description: SQL 작성없이 User를 수정할 수 있는 Operator에 대해 설명한다.
---

# Edit User GUI Operator

## User Interface

Edit User 를 선택하면, 아래와 같이 User 정보를  설정하는 창이 열린다.

<figure><img src="../../../../../.gitbook/assets/image (48).png" alt="" width="375"><figcaption><p>Edit User</p></figcaption></figure>

* 각 Edit User 의 각 탭에서 생성시 설정할 수 있는 다양한 옵션이 있으며 자세한 설명은 다음과 같다.

<table><thead><tr><th width="169">항목</th><th>설명</th></tr></thead><tbody><tr><td>Info</td><td>사용자 PW 등 다양한 정보를 수정한다. </td></tr><tr><td>Role</td><td>사용자에게 주어진 Role 을 수정한다.</td></tr><tr><td>System Privilege</td><td>사용자에게 주어지는 시스템 권한을 수정한다.</td></tr><tr><td>Object Privilege</td><td>사용자에게 주어진 오브젝트 권한을 수정한다.</td></tr><tr><td>Quota</td><td>테이블스페이스 사이즈를 수정한다.</td></tr></tbody></table>

### Info

<figure><img src="../../../../../.gitbook/assets/image (45).png" alt="" width="375"><figcaption><p>Edit User - Info tab</p></figcaption></figure>

Info 탭에서는 유저의 비밀 번호 등을 변경할 수 있으며, 각 항목에 대한 설명은 다음과 같다.

<table><thead><tr><th width="199">항목</th><th>설명</th></tr></thead><tbody><tr><td>User Name</td><td>사용자 이름을 나타내며 변경이 불가하다.</td></tr><tr><td>New Password</td><td>패스워드 변경시 새로운 패스워드를 입력한다.</td></tr><tr><td>Confirm Password</td><td>패스워드 변경시 새로운 패스워드를 다시한번 입력한다.</td></tr><tr><td>Password Expired</td><td>사용자의 패스워드를 사용기간 만료 상태로 생성하여, 해당 사용자가 처음 접속 시 패스워드를 입력할 수 있도록 한다.</td></tr><tr><td>Account Lock</td><td>사용자 생성 시 잠금상태로 생성한다.</td></tr><tr><td>More Option</td><td>자세한 내용은 CREATE USER - MORE OPTIONS 참고한다.</td></tr><tr><td>Reset</td><td>기존의 설정 항목들을 초기화 한다.</td></tr></tbody></table>

### Role

<figure><img src="../../../../../.gitbook/assets/image (46).png" alt="" width="375"><figcaption><p>Edit User - Role Tab</p></figcaption></figure>

Role 탭에서는 사용자에게  부여된 롤을 확인하고 새로운 롤을 부여하거나 해당 롤을 회수할 수 있다. 각 항목의 설명은 다음과 같다.

<table><thead><tr><th width="250">항목</th><th>설명</th></tr></thead><tbody><tr><td>Granted Role List</td><td><p>현재 사용자가 소유한 Role의 목록을 보여준다.</p><ul><li>Role : 현재 부여받은 Role의 이름을 보여준다.</li><li>Admin : 다른 사용자에게 Role을 부여할 수 있다.</li><li>Default : 사용자가 접속시 Role을 활성화 한다.</li><li>Revoke : 회수할 Role을 선택한다.</li><li>Edit 버튼 클릭시 수행된다.</li></ul></td></tr><tr><td>Added Role List</td><td><p>현재 사용자에게 추가할 Role의 리스트를 보여준다.</p><ul><li>+ : Add Role 창을 띄운다.<br>Add Role을 통해 사용자에게 부여할 Role을 추가한다.</li><li>- : 선택된 Role 리스트를 삭제한다.</li></ul></td></tr></tbody></table>



### System Privilege

<figure><img src="../../../../../.gitbook/assets/image (47).png" alt="" width="375"><figcaption><p>Edit User - System Privilege Tab</p></figcaption></figure>

System Privilege 탭에서는 사용자에게 시스템 권한을 부여/회수할 수 있으며, 자세한 설명은 다음과 같다.

<table><thead><tr><th width="253">항목</th><th>설명</th></tr></thead><tbody><tr><td>Granted System Privilege</td><td><p>사용자가 소유한 시스템 권한 목록을 보여준다.</p><ul><li>System Privilege : 시스템 권한 이름을 보여준다.</li><li>Admin : 다른 사용자에게도 권한을 부여할 수 있다.</li><li>Revoke : 회수할 Role을 선택한다.</li><li>Edit 버튼 클릭시 수행된다.</li></ul></td></tr><tr><td>Added System Privilege</td><td><p>사용자에게 추가할 시스템 권한 목록을 보여준다.</p><ul><li>+: Add System Privilege 창을 띄운다.<br>Add System Privilege를 통해 사용자/롤에 부여할 시스템 권한을 추가한다.</li><li>- : 선택된 System 권한 목록을 삭제한다.</li></ul></td></tr></tbody></table>



### Object Privilege

<figure><img src="../../../../../.gitbook/assets/image (40).png" alt="" width="375"><figcaption><p>Edit User - Object Privilege</p></figcaption></figure>

Object Privilege 탭에서는 사용자에게 오브젝트 권한을 부여/회수할 수 있으며, 자세한 설명은 다음과 같다.

<table><thead><tr><th width="232">항목</th><th>설명</th></tr></thead><tbody><tr><td>Granted Object Privilege</td><td><p>사용자가 소유한 오브젝트 권한 목록을 보여준다.</p><ul><li>Schema, Object Type, Object Name : 권한 대상 오브젝트를 나타낸다.</li><li>Privilege : 해당 오브젝트에 대한 권한을 보여준다.</li><li>Admin : 다른 사용자에게도 권한을 부여할 수 있다.</li><li>Revoke : 회수할 Role을 선택한다.</li><li>Edit 버튼 클릭시 수행된다.</li></ul></td></tr><tr><td>Added Object Privilege</td><td><p>사용자에게 추가할 시스템 권한 목록을 보여준다.</p><ul><li>+: Add Object Privilege 창을 띄운다.<br>Add Object Privilege를 통해 사용자에 부여할 오브젝트 권한을 추가한다.</li><li>- : 선택된 Object 권한 목록을 삭제한다.</li></ul></td></tr></tbody></table>

### Quota

<figure><img src="../../../../../.gitbook/assets/image (41).png" alt="" width="375"><figcaption></figcaption></figure>

Quota 탭에서는 사용자가 사용 가능한 테이블스페이스의 사이즈를 설정할 수 있다.&#x20;
