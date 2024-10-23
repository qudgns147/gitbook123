# Schema

#### 3.1.2. Schema Object Detail <a href="#d5e2089" id="d5e2089"></a>

Schema Tree Browser에서 스키마 객체를 선택하면, **View 영역**의 **Schema Object Detail 화면**에서 스키마 객체의 세부 정보를 조회할 수 있다. 선택한 스키마 종류에 따라 탭이 다르게 구성되며, 선택한 스키마 객체명이 Schema Object Detail의 Title 이름이 된다.

다음은 객체명이 CONTRACT인 Table 객체를 클릭했을 때의 화면이다. Table 객체의 경우 컬럼, 제약조건, 데이터, 인덱스, 파티션 등의 정보를 확인할 수 있다.

\[그림 3.6] Schema Object Detail 화면

| ![Schema Object Detail 화면](https://technet.tmax.co.kr/upload/download/online/tibero/pver-20170425-000001/user-guide/resources/figure\_obj\_details.png) |
| ------------------------------------------------------------------------------------------------------------------------------------------------------- |

\


**Schema Tree Browser**의 **Object List**를 클릭하면 해당 오브젝트의 상세 정보를 확인할 수 있으며, 오른쪽 마우스 버튼을 클릭하면 일반적으로 다음과 같은 기능을 사용할 수 있다.

*   **Database Object**

    Schema Tree Browser의 최상위 노드로 데이터베이스 연결 단위(Session)로 생성되는 오브젝트이다.

    **\[Database] > \[Detail View]**를 선택하면 다음의 탭으로 구성된 화면이 나타난다.

    | 탭                    | 설명                             |
    | -------------------- | ------------------------------ |
    | **\[Info]**          | 데이터베이스 정보를 조회한다.               |
    | **\[Instance]**      | 데이터베이스 인스턴스 정보를 조회한다.          |
    | **\[Version]**       | 데이터베이스 버전 정보를 조회한다.            |
    | **\[Shared Memory]** | 데이터베이스 Shared Memory 정보를 조회한다. |
    | **\[Sessions]**      | 데이터베이스 세션정보를 조회한다.             |
*   **Schema Object**

    데이터베이스의 하위노드로, Public과 유저 목록으로 구성되는 오브젝트이다.

    **\[Schema] > \[Detail View]**를 선택하면 다음의 탭으로 구성된 화면이 나타난다.

    | 탭                        | 설명                                  |
    | ------------------------ | ----------------------------------- |
    | **\[Info]**              | 스키마(유저) 정보를 조회한다.                   |
    | **\[Role Grants]**       | 스키마가 보유한 Role 목록을 조회한다.             |
    | **\[System Privileges]** | 스키마가 보유한 System Privilege 목록을 조회한다. |
    | **\[Object Grants]**     | 스키마가 보유한 Object Grant 목록을 조회한다.     |
    | **\[Objects]**           | 스키마가 보유한 Object 목록을 조회한다.           |
    | **\[Extents]**           | 스키마가 보유한 Extent 목록을 조회한다.           |
    | **\[Script]**            | 스키마의 Script 정보를 출력한다.               |
