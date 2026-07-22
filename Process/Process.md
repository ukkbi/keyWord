# Process

메모리에 로드되어 CPU를 할당받아 실행 중인 프로그램

디스크에 정적인 파일 형태로 존재할 때는 프로그램

프로그램이 메모리에 올려져 OS에 의해 관리되며 돌아가기 시작하면 프로세스

<img src = "../img/process.png" width = "400" height = "250"></image>

## 특징

- 독립된 메모리 구조
    - code : 작성한 커스텀 코드 및 기계어 명령저 저장
    - Data : 전역 변수, 정적 변수 저장
    - Heap : 개발자가 동적 할당 하는 영역
    - Stack : 지역 변수, 매개 변수, 함수 호출 시의 돌아갈 리턴 주소 저장
- OS의 관리 단위
    - [PCB](PCB(ProcessControlBlock).md)를 통해 OS 커널에 의해 관리됨
    - 각 프로세스는 고유한 [PID](PCB-ProcessId.md)를 할당 받음