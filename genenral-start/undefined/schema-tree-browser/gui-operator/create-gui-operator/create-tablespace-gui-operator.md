---
description: SQL 작성없이 Tablespace를 생성할 수 있는 Operator에 대해 설명한다.
---

# Create Tablespace GUI Operator

## User Interface

Schema Tree > Context Menu > Create Tablespace 를 선택하면, 아래와 같이 테이블스페이스를 생성할 수 있는 창이 열린다.

<figure><img src="../../../../../.gitbook/assets/image (63).png" alt="" width="375"><figcaption><p>Create Tablespace UI</p></figcaption></figure>

Create View의 각 탭에서 테이블 생성시 설정할 수 있는 다양한 옵션이 있으며 자세한 설명은 다음과 같다

* Create View Tab List

<table><thead><tr><th width="160">항목</th><th>설명</th></tr></thead><tbody><tr><td>Common</td><td>Tablespace의 이름 등 기본적인 정보를  설정한다.</td></tr><tr><td>File Setting</td><td>테이블스페이스에 대한 세부 사항을 설정한다.</td></tr><tr><td>Options</td><td>추가적인 옵션을 설정한다.</td></tr></tbody></table>

### Common

<figure><img src="../../../../../.gitbook/assets/image (63).png" alt="" width="375"><figcaption><p>Create Tablespace Common </p></figcaption></figure>

<table><thead><tr><th width="160">항목</th><th>설명</th></tr></thead><tbody><tr><td>Name</td><td>테이블스페이스 이름을 설정한다.</td></tr><tr><td>Type</td><td><p>테이블 스페이스 타입을 설정한다.</p><ul><li>PERMANENT : 테이블스페이스를 생성한다.</li><li>TEMP : 임시 테이블스페이스를 생성한다.</li><li>UNDO : Undo 테이블스페이스를 생성한다.</li></ul></td></tr></tbody></table>

### File Setting

File Setting 탭에서는 파일의 세부사항들을 설정한다.

<figure><img src="../../../../../.gitbook/assets/image (132).png" alt="" width="375"><figcaption><p>Create Tablespace File Setting</p></figcaption></figure>

* 각 항목에 대한 설명은 다음과 같다.

<table><thead><tr><th width="241">항목</th><th>설명</th></tr></thead><tbody><tr><td>File Specification List</td><td><p>생성할 파일 목록을 나타낸다.</p><p>+/-버튼을 통해 파일을 추가/삭제한다.</p></td></tr><tr><td>File Name</td><td>테이블 스페이스 파일 이름을 설정한다.</td></tr><tr><td>Directory</td><td>파일이 저장될 경로를 설정한다.</td></tr><tr><td>File Size</td><td>파일의 사이즈를 설정한다.</td></tr><tr><td>Reuse</td><td>기존의 파일이 있을 때 덮어쓸지의 여부를 지정한다.</td></tr><tr><td>Auto Extent</td><td>저장할 데이터가 파일 크기를 초과할 경우 자동으로 파일을 늘려준다.</td></tr><tr><td> Next</td><td>파일의 크기를 확장할 때 늘어나는 크기를 지정할 수 있다.</td></tr><tr><td>Max Size</td><td>파일 크기의 최댓값을 지정할 수 있다. </td></tr></tbody></table>

### Options

Option 탭에서는 File 외 Tablespace에 대한 추가적인 옵션을 설정한다.

<figure><img src="../../../../../.gitbook/assets/image (133).png" alt="" width="375"><figcaption><p>Options Tab</p></figcaption></figure>

* 각 항목에 대한 설명은 다음과 같다.

<table><thead><tr><th width="258">항목</th><th>설명</th></tr></thead><tbody><tr><td>Uniform Extent</td><td>Extent의 크기를 사용자가 설정한다.</td></tr><tr><td>Tablespace Encryption</td><td>테이블스페이스를 암호화한다.</td></tr><tr><td>Logging</td><td>오브젝트에 대한 작업을 Redo Log로 기록한다.</td></tr><tr><td>Force Logging</td><td>No Logging 상태로 바뀌더라도 Logging 된다.</td></tr><tr><td>Online</td><td>테이블스페이스를 온라인 상태로 생성한다.</td></tr></tbody></table>
