---
description: 본 절에서는 Tibero Studio에 로그인하기 위한 정보와 데이터베이스 서버 정보를 설정한 후 접속하고 종료하는 방법에 대해서 설명한다.
---

# Connection (접속 및 종료)

## 로그인 설정과 데이터베이스 접속 <a href="#sect_dbs_connect" id="sect_dbs_connect"></a>

Tibero Studio 바이너리 실행 파일을 실행하면, 데이터베이스 서버에 접속하기 위해 필요한 정보를 설정하는 **Login & Connection Config 화면**이 나타난다.

Tibero Studio를 통해 데이터베이스 서버에 접속하는 방법은 다음과 같다.

1.  **Login & Connection Config 화면**의 각 항목에 접속할 데이터베이스 서버의 로그인 정보를 입력한다.



    <figure><img src="../../.gitbook/assets/image (87).png" alt=""><figcaption><p>[그림 1.1] Login &#x26; Connection Config 화면</p></figcaption></figure>



    *   **입력 항목**

        <table><thead><tr><th width="208">항목</th><th>설명</th></tr></thead><tbody><tr><td>Alias</td><td>접속 정보를 나타내는 이름을 입력한다.</td></tr><tr><td>IP</td><td>데이터베이스 서버의 IP 주소를 입력한다.</td></tr><tr><td>Port</td><td>데이터베이스 서버의 포트 번호를 입력한다. Tibero를 설치할 때 별도의 포트 번호를 지정하지 않았다면, 디폴트로 지정되는 포트 번호는 8629이다.</td></tr><tr><td>User</td><td>접속할 데이터베이스의 사용자 이름을 입력한다.</td></tr><tr><td>Password</td><td>접속할 데이터베이스의 사용자 패스워드를 입력한다. 오른쪽의 <strong>'Save'</strong> 체크박스를 체크하면 입력한 패스워드를 저장할 수 있다. 패스워드를 저장하면 다음에 접속할 때 패스워드를 다시 입력하지 않아도 된다.</td></tr><tr><td>DB Name</td><td>SID를 입력한다. Tibero를 설치할 때 별도의 SID를 지정하지 않았다면, 디폴트로 지정되는 SID는 'tibero'로 설정된다.</td></tr><tr><td>Connection Time</td><td>접속 시 대기시간을 설정한다.</td></tr><tr><td>Color</td><td>연결정보마다 색 지정할 수 있다.</td></tr><tr><td>SSL</td><td>서버와 클라이언트 간의 데이터 통신을 암호화한다.</td></tr></tbody></table>
    *   **버튼**

        | 버튼             | 설명                                                              |
        | -------------- | --------------------------------------------------------------- |
        | **\[Delete]**  | 선택한 로그인 정보를 삭제한다.                                               |
        | **\[Import]**  | 데이터베이스 접속을 위해 기존에 xml 파일로 만들어진 로그인 정보를 가져온다.                    |
        | **\[Export]**  | 데이터베이스 접속을 위해 만들어진 로그인 정보를 xml 파일로 내보낸다. 단, Password는 저장되지 않는다. |
        | **\[New]**     | 데이터베이스에 접속하기 위한 새로운 로그인 정보를 만든다.                                |
        | **\[Save]**    | 입력한 로그인 정보를 등록한다.                                               |
        | **\[Cancel]**  | **Login & Connection Config 화면**을 닫는다.                          |
        | **\[Test]**    | 입력한 로그인 정보로 데이터베이스에 정상으로 접속되는지 테스트한다.                           |
        | **\[Connect]** | 등록된 데이터베이스 서버에 접속을 요청한다.                                        |
2. 입력된 로그인 정보가 맞는지 테스트하려면 **\[Test]** 버튼을 클릭한다. 테스트 없이 새로운 로그인 정보를 등록하려면 **\[Save]** 버튼을 클릭한다. 기존의 로그인 정보를 수정한 후 새로 등록하려면 **\[Save As]** 버튼을 클릭한다.
3.  **Login & Connection Config 화면**에 각 입력 항목을 입력한 뒤 **\[Connect]** 버튼을 클릭했을 때 데이터베이스 서버에 정상적으로 접속되면 다음과 같은 초기 화면이 나타난다.



    <figure><img src="../../.gitbook/assets/image (86).png" alt=""><figcaption><p>[그림 n.1] 초기화면</p></figcaption></figure>

    \


    #### 참고

    초기 화면에 대한 자세한 내용은 ["User interface"](user-interface.md)을 참고한다.

## 종료 <a href="#d5e353" id="d5e353"></a>

Tibero Studio를 종료하려면 **\[File] > \[Exit]** 메뉴를 선택하거나 오른쪽 상단의 **\[x]** 버튼을 클릭한다.
