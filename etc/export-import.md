# Export / Import

메뉴에서 **\[Tool] > \[Import from file]** 또는 **\[Tool\[] > \[Export to file]**을 선택하면 파일로 데이터베이스 테이블의 데이터를 추출하거나 입력할 수 있다.

#### 3.6.1. Import from file <a href="#d5e1899" id="d5e1899"></a>

메뉴에서 **\[Tool] > \[Import from file]** 을 선택하면 **Import from file 화면**에서 파일의 데이터를 데이터베이스 테이블의 데이터로 입력할 수 있다.

Import to file 화면은 **File Options, Destination table, Status/Log, Setting Import Options, Column List Editor** 로 구성된다.

\[그림 3.28] Import from file 화면

| ![Import from file 화면](https://technet.tmax.co.kr/upload/download/online/tibero/pver-20230906-000001/user-guide/resources/figure\_import\_from\_file.png) |
| --------------------------------------------------------------------------------------------------------------------------------------------------------- |

\


*   **File Options**

    | 항목                      | 설명                                            |
    | ----------------------- | --------------------------------------------- |
    | Source file             | Import 할 파일의 경로를 설정한다.                        |
    | Destination table       | 파일의 내용을 삽입할 테이블을 설정한다.                        |
    | Delete before a loading | 기존 테이블의 데이터를 Delete하고 Import 할지 설정한다.         |
    | Truncated before a load | 기존 테이블의 데이터를 Truncate하고 Import 할지 설정한다.       |
    | Ignore the first line   | 파일의 첫 번째 라인(Column header)을 무시할지 설정한다.        |
    | Remove trailing spaces  | 데이터의 문자열 끝의 불필요한 space를 제거한다.                 |
    | One Transaction         | Import 작업 전체가 끝났을 때 Commit 할지 설정한다.           |
    | Save log                | Import 작업의 로그를 파일로 저장할지 설정한다.                 |
    | Batch Execution         | Import 작업을 배치(batch)로 실행할지 설정하고, 배치 단위를 설정한다. |
*   **Destination table**

    \[그림 3.29] Destination table 화면

    | ![Destination table 화면](https://technet.tmax.co.kr/upload/download/online/tibero/pver-20230906-000001/user-guide/resources/figure\_destination\_table.png) |
    | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |

    \


    파일의 내용을 삽입할 테이블을 선택한다.

    현재 연결된 데이터 베이스의 User별 테이블이 트리형태로 나타난다. 테이블의 이름을 검색할 수 있으며, Full Match 옵션을 선택할 경우 검색 내용과 완전히 일치하는 테이블만 나타난다.
*   **Status/Log**

    Import 상태와 로그를 조회한다.
*   **Setting Import Options**

    \[그림 3.30] Setting Import Options 화면

    | ![Setting Import Options 화면](https://technet.tmax.co.kr/upload/download/online/tibero/pver-20230906-000001/user-guide/resources/figure\_setting\_import\_options.png) |
    | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |

    \


    | 항목                      | 설명                                          |
    | ----------------------- | ------------------------------------------- |
    | Field Delimiter         | 각 필드를 구분할 구분자(Delimiter)를 설정한다.             |
    | Field Qualifier         | 각 필드를 감쌀 수식어(Qualifier)를 설정한다.              |
    | Record Delimiter        | 각 레코드를 구분할 구분자를 설정한다.                       |
    | Import Date Format      | 테이블에 삽입할 파일 데이터의 DATE 형식 Format을 입력한다.      |
    | Import Timestamp Format | 테이블에 삽입할 파일 데이터의 Timestamp 형식 Format을 입력한다. |
*   **Column List Editor**

    Column List Editor 에서 테이블의 Column에 맞게 파일 데이터의 Column을 편집할 수 있다.

    \[그림 3.31] Column List Editor 화면

    | ![Column List Editor 화면](https://technet.tmax.co.kr/upload/download/online/tibero/pver-20230906-000001/user-guide/resources/figure\_column\_list\_editor.png) |
    | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |

    \


    **Column List** 는 선택한 테이블의 Column들을 나타내고, **Data Sample From File** 은 파일 데이터의 Column 들을 나타낸다.

    Data Sample From File의 항목을 드래그하여 순서를 편집할 수 있고, 선택 후 **\[Delete] 버튼**을 클릭하여 삭제할 수 있다.

#### 3.6.2. Export to file <a href="#d5e2019" id="d5e2019"></a>

메뉴에서 **\[Tool] > \[Export ti file]** 을 선택하면 **Export to file 화면**에서 데이터베이스 테이블의 데이터를 파일로 추출할 수 있다.

\[그림 3.32] Export to file 화면

| ![Export to file 화면](https://technet.tmax.co.kr/upload/download/online/tibero/pver-20230906-000001/user-guide/resources/figure\_export\_to\_file.png) |
| ----------------------------------------------------------------------------------------------------------------------------------------------------- |

\


| 항목             | 설명                                                                              |
| -------------- | ------------------------------------------------------------------------------- |
| Table          | 파일로 추출할 테이블을 선택한다.                                                              |
| SQL Query      | 테이블의 데이터를 조회하는 쿼리이다. Custom 옵션을 선택할 경우, 쿼리를 직접 작성하여 사용자가 원하는 데이터만을 추출할 수 있다.    |
| File Directory | 데이터가 저장될 파일을 선택한다. Include Header Line 옵션을 선택할 경우, 테이블의 Column을 포함해서 데이터가 저장된다. |

*   **Status/Log**

    Export 상태와 로그를 조회한다.
*   **Setting Export Options**

    \[그림 3.33] Setting Export Options 화면

    | ![Setting Export Options 화면](https://technet.tmax.co.kr/upload/download/online/tibero/pver-20230906-000001/user-guide/resources/figure\_setting\_export\_options.png) |
    | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |

    \


    | 항목                      | 설명                                      |
    | ----------------------- | --------------------------------------- |
    | Field Delimiter         | 각 필드를 구분할 구분자(Delimiter)를 설정한다.         |
    | Field Qualifier         | 각 필드를 감쌀 수식어(Qualifier)를 설정한다.          |
    | Record Delimiter        | 각 레코드를 구분할 구분자를 설정한다.                   |
    | Export Date Format      | 파일에 저장될 데이터의 DATE 형식 Format을 입력한다.      |
    | Export Timestamp Format | 파일에 저장될 데이터의 Timestamp 형식 Format을 입력한다. |
