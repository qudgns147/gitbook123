# Installation

### 제2장 설치 및 기동

본 장에서는 Tibero Studio 설치 및 기동 방법, 파라미터 설정에 대해 설명한다.

### 2.1. 설치 및 기동 <a href="#d5e214" id="d5e214"></a>

Tibero Studio는 별도의 설치 과정 없이 사용자 PC 플랫폼에 맞는 Tibero Studio의 압축 파일을 해제하고 바이너리 실행파일을 실행시키면 바로 기동한다. 설치용 압축 파일의 경로 정보는 [“1.3. 설치 전 준비사항”](https://technet.tmax.co.kr/upload/download/online/tibero/pver-20170425-000001/installation-guide/chapter\_overview.html#sect\_preparation\_install)을 참고한다.

다음은 Tibero Studio를 설치하고 기동하는 과정에 대한 설명이다.

1. 사용자 PC 플랫폼에 맞는 Tibero Studio의 압축 파일을 다운로드 받는다.
   *   UNIX 계열(LINUX 포함)

       | 파일명                      | 설명                                  |
       | ------------------------ | ----------------------------------- |
       | linux.gtk.x86.tar.gz     | 설치할 플랫폼이 32bit일 때 실행할 수 있는 압축 파일이다. |
       | linux.gtk.x86\_64.tar.gz | 설치할 플랫폼이 64bit일 때 실행할 수 있는 압축 파일이다. |
   *   Windows 계열

       | 파일명                     | 설명                                  |
       | ----------------------- | ----------------------------------- |
       | win32.win32.x86.zip     | 설치할 플랫폼이 32bit일 때 실행할 수 있는 압축 파일이다. |
       | win32.win32.x86\_64.zip | 설치할 플랫폼이 64bit일 때 실행할 수 있는 압축 파일이다. |
2.  다운로드받은 Tibero Studio 압축 파일을 원하는 디렉터리에 해제한다.

    기존에 Tibero Studio가 설치된 경로가 있다면 삭제해야 하고, 디렉터리 경로에는 특수문자가 없어야 한다(Linux의 경우 공백 또는 특수문자(\\, /, :, \*, ?, ", <, >, | 등)가 포함된 파일 삭제가 어려울 수 있으므로 주의한다).
3.  다음은 압축 파일을 해제한 구조이다. 해당 파일과 경로가 정상적으로 해제되어 있는지 확인한다.

    ```
    +- linux.gtk.x86
       |
       +- TiberoStudio.exe
       |
       +- TiberoStudio.ini
       |
       +- plugins
       |
       +- configuration
       |
       +- lib
       |
       +- ...
    ```

    #### 참고

    압축 파일의 구조는 Linux(32bit/64bit), Window(32bit/64bit) 모두 동일하다.
4. 압축 파일을 해제한 경로에 **TiberoStudio.exe** 바이너리 파일을 실행하면 Tibero Studio가 기동된다.

### 2.2. 파라미터 설정 <a href="#d5e269" id="d5e269"></a>

바이너리 실행파일이 위치하고 있는 디렉터리의 **TiberoStudio.ini** 파일에서 메모리와 관련된 파라미터를 조정할 수 있다. 예를 들어 사용 메모리가 늘어나서 프로그램이 느려지면 Heap 사이즈의 크기를 최대로 설정해서 Tibero Studio의 성능을 향상시킬 수 있다. 따로 조정하지 않으면 디폴트 값이 적용된다.

다음은 각 항목에 대한 설명이다.

\<TiberoStudio.ini >

```
-vmargs
-xms256m
-xmx512m
-XX:PermSize=int
-XX:MaxPermSize=int
-XX:NewSize=int
```

| 항목             | 설명                                       |
| -------------- | ---------------------------------------- |
| xms256m        | Heap 사이즈 최소 크기이다. (기본값: 256)             |
| xmx512m        | Heap 사이즈 최대 크기이다. (기본값: 512, 최댓값: 1024)  |
| XX:PermSize    | Permanent Generation 크기이다. (기본값: 128)    |
| XX:MaxPermSize | Permanent Generation 최대 크기이다. (기본값: 256) |
| XX:NewSize     | New Generation 크기이다. (기본값: 128)          |

다음은 설정 예이다.

```
-vmargs
-xms256m
-xmx512m
-XX:PermSize=128m
-XX:MaxPermSize=128m
-XX:NewSize=128m
```

**\[참고]**

메모리가 부족으로 기동 시 에러가 발생한다면, TiberoStudio 설치된 폴더 안에 있는 **TiberoStudio.ini** 파일에 Xms, Xmx 값을 수정한다.

* 기본값 : -Xms256m -Xmx512m
* RAM 1G : -Xms128m -Xmx256m
* RAM 2G : -Xms256m -Xmx512m
* RAM 2G 이상 : -Xms512m -Xmx1024m
