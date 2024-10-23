# Recompile Invalid Object

## User Interface

메뉴에서 \[View] > \[Tools] > \[Recompile Invalid Object]를 선택하면 Recompile Invalid Object 화면에서 유효하지 않은 객체(Invalid Object)를 일괄로 컴파일할 수 있다. 화면은 Object Find 영역과 Find Result , Recompile Result 영역으로 구성된다.

<figure><img src="../../../.gitbook/assets/image (148).png" alt="" width="375"><figcaption><p>Recompile Invalid Object 초기화면</p></figcaption></figure>

### **Object Find 영역**

Object Find 영역에서는 유효하지 않은 객체를 탐색하는 조건을 설정할 수 있다.&#x20;

<table><thead><tr><th width="231">항목</th><th>설명</th></tr></thead><tbody><tr><td>Connection</td><td>컴파일 할 대상이 속한 연결정보를 선택한다.</td></tr><tr><td>Schema</td><td>컴파일 할 대상의 스키마를 선택한다.</td></tr><tr><td>Object Type</td><td>컴파일 할 대상의 타입이다.</td></tr><tr><td>Reset</td><td>설정 및 결과창 모두를 초기화한다.</td></tr><tr><td>Find Invalid Object</td><td>유효하지 않은 객체를 검색한다.</td></tr></tbody></table>

### Find Result

Object Find 영역에서 정의한 조건에 따라 Find 탐색된 Object 리스트를 보여준다.

<figure><img src="../../../.gitbook/assets/image (149).png" alt="" width="375"><figcaption><p>Find Object Result</p></figcaption></figure>

각 항목에 대한 설명은 다음과 같다.

<table><thead><tr><th width="208">항목</th><th>설명</th></tr></thead><tbody><tr><td>Check Box</td><td>컴파일 할 대상을 선택한다.</td></tr><tr><td>Object Type</td><td>컴파일 할 대상의 타입을 나타낸다.</td></tr><tr><td>Count</td><td>각 오브젝트 별 개수를 나타낸다.</td></tr><tr><td>Object Name</td><td>오브젝트 이름을 나타낸다.</td></tr><tr><td>Status</td><td>현재 오브젝트의 상태를 나타낸다.</td></tr></tbody></table>

### Recompile Result

Find Result에서 Recompile을 수행할 경우 다음과 같이 Recompile Invalid Object에서 Recompile 결과를 볼 수 있다.&#x20;

<figure><img src="../../../.gitbook/assets/image (150).png" alt="" width="375"><figcaption><p>Recompile Result > Summary</p></figcaption></figure>

* Summary는Recompile 결과를  Object 타입별로 요약하여 결과를 제공한다.&#x20;
* Detail에서는 Recompile 대상 별 Recompile 성공여부를 나타낸다.&#x20;



다음은 Compile Invalid Objects 화면을 사용하는 절차이다.

1. 컴파일할 대상 연결정보를 Connection 항목에서 선택한다.
2. 컴파일할 대상 스키마를 **'Schema'** 항목에서 선택한다.
3. 컴파일할 대상 타입을 **'Type'** 항목에서 중에서 선택한다.
4. **\[Find Invaild Objects]** 버튼을 클릭하여 **\[Invalid Object List]** 탭의 내용을 업데이트한다.
5. **\[Object List]** 탭에서 원하는 객체를 선택한 후 **\[Recompile]** 버튼을 클릭한다.
6. 자세한컴파일한 결과를 보기 위해서 **\[Detail] 을** 선택하여  각 오브젝트별  컴파일 결과를 확인한다.

