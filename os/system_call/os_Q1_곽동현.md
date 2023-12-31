### 1. 시스템 콜이 무엇인지 설명해주세요.

시스템 콜은 `커널모드`와 `사용자모드`간에 필요한 정보를 주고받기 위해 호출하는 함수입니다.
운영체제는 중요 자원을 보호하기 위해 커널모드와 사용자모드 2가지로 구분하기 되어 있습니다.
프로세스에서 필요한 자원에 접근해서 작업을 처리해야 할 때, 시스템 콜을 사용하여 필요한 요청을 하고 이에따른 결과값을 돌려받게 됩니다.

### 2. 우리가 사용하는 시스템 콜의 예시를 들어주세요.

저희가 사용하는 자바에서는 native 인터페이스로 활용하여 파일을 읽을 때 시스템 콜이 사용될 수 있습니다.
자바는 JVM이 존재하기 때문에 버퍼에 실어서 커널모드와 데이터를 주고받습니다.

### 3. 시스템 콜의 유형에 대해 설명해 주세요.

시스템 콜의 유형으로는 크게 6가지로 분류할 수 있습니다.
`프로세스 제어`, `파일 조작`, `장치 관리` , `정보 유지` , `통신` , `보호`의 유형이 있습니다.

### 4. 운영체제의 Dual Mode 에 대해 설명해 주세요.

운영체제에서 사용자로부터 자원을 안전하게 보호하기 위해서 나눈 2개의 모드입니다.
`사용자모드`와 `커널모드`로 구분되어 있습니다.

### 5. 왜 유저모드와 커널모드를 구분해야 하나요?

유저모드와 커널모드를 구분하지 않고 유저가 자유롭게 운영체제의 자원을 가져다 쓴다면은, 시스템 자체가 망가질 수 있습니다.
이에 따라 사용자 모드에서는 커널 모드의 자원을 접근할 수 없도록 제한을 두고 있습니다.

### 6. 서로 다른 시스템 콜을 어떻게 구분할 수 있을까요?

커널은 각각 시스템 콜을 구분하기 위해 각각 고유번호를 할당하고, 번호에 해당하는 제어루틴을 커널 내부에 정의합니다.
커널은 요청받은 시스템 콜의 번호를 확인한 후, 그 번호에 맞는 서비스 루틴을 호출하게 됩니다.



---
### 운영체제란 무엇인가요?

시스템의 자원과 동작들을 관리하는 소프트웨어입니다. 
주로 프로세스(프로그램),네트워크,저장장치,하드웨어,사용자와 같은 5가지를 관리합니다.

