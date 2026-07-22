# CPU register

CPU 내부의 데이터를 임시로 저장하는 **최고속의 초소형 기억장치**
**메모리 계층 구조의 최상단**에 위치함
CPU가 지금 당장 연산하거나 처리해야 하는 데이터와 명령어를 저장함

## 특징

- 압도적 속도 : SRAM 기반인 L1/L2 Cache나 DRAM 기반인 메인 메모리보다 훨씬 빠르며,
CPU의 클럭 주기와 동일한 속도로 동작함
- 적은 용량 & 높은 단가 : 회로 구조가 복잡하고 칩 면적을 많이 차지하여 용량이 매우 작음

## **주요 레지스터 종류**

- **PC (Program Counter):** 다음에 실행할 명령어의 메모리 주소를 저장.
- **IR (Instruction Register):** 현재 실행 중인 명령어를 저장.
- **ACC (Accumulator / 누산기):** ALU(산술논리연산장치)의 연산 결과를 임시 저장.
- **MAR (Memory Address Register):** 읽거나 쓸 메모리의 주소를 저장.
- **MBR / MDR (Memory Buffer/Data Register):** 메모리에서 읽어오거나 쓸 실제 데이터를 저장.
- **SP (Stack Pointer):** 현재 스택 영역의 최상단 주소를 지칭