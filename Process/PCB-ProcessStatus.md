# [PCB](PCB(ProcessControlBlock).md) - Process Status

프로세스가 어떤 상태에 있는지, CPU와 메모리를 얼마나 사용하고 있는지, 어떤 자원을 점유하고 있는지 등 실행 현황 전체를 종합해서 나타내는 정보

<img src="../img/PCB - Process Status.png" width = 300 height = 200></image>

## 특징

종합적인 현황판 : 단순히 “실행 중이다/ 대기 중이다”(Process State) 하는 단편적인 단계를 넘어,  
PID, CPU/메모리 점유율, 소유계정, 실행 명령어 등 프로세스에 관한   
제어 관리용   데이터가 묶여 있는 개념