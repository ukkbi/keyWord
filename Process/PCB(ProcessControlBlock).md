# PCB(Process Control Block)

운영체제가 프로세스를 관리하기 위해 프로세스의 상태 및 제어 정보를 저장하는 데이터 구조

<img src="../img/PCB.png" width = 400 height = 250></image>

## 특징

프로세스가 생성될 때 커널 영역에 생성됨, 프로세스 종료시 함께 파기

문맥 교환의 핵심 : CPU가 실행 중인 프로세스를 중단하고 다른 프로세스로 전환할 때
현재 프로세스의 작업 상태를 해당 프로세스의 PCB에 저장하고 
새로 실행할 프로세스의 PCB에서 상태를 복원함

커널 영역 : 일반 사용자가 임의로 변경하지 못하도록 운영체제의 보호된 메모리 영역
이 커널 영역 내의 Process Table 현태로 관리된다

## PCB에 저장되는 주요 정보

1. [PID](PCB-ProcessId.md) (Process ID) : 프로세스 식별 번호
2. [Process State](PCB-ProcessStatus.md) : 생성(new) , 준비 (ready), 실행(Running), 대기(waiting), 종료(terminated)
3. [Program Counter](PCB-PC.md)(PC) : 프로세스가 다음에 실행할 명령어의 메모리 주소
4. [CPU Registers](CPURegister.md) : acumulator, index register, stack pointer 등의 레지스터 상태 값
5. CPU scheduling information : 우선 순위, 큐 포인터 등
6. Memory Management Information : Page table, Segment table 정보
7. Accouting & I/O Status : CPU 사용시간, 열린 파일 목록(file Descriptor) 등