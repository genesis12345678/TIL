# 모드 스위치와 프로세스 스위치의 차이는 무엇인가요?

- **모드 스위치**는 사용자 모드에서 커널 모드로 변경할 때 발생하며, 완전 문맥 교환이 필요하지 않고 시스템 스택을 사용한다.
- **프로세스 스위치**는 보통 문맥 교환(Context Switching)이라고 하며, 실행 중인 프로세스를 멈추고 새 프로세스를 실행하는 것이다.

### Context Switching이 발생하는 경우 3가지
1. **멀티 태스킹**
   - 실행 가능한 프로세스들이 운영체제의 스케줄러에 의해 **조금씩 번갈아가며** 수행되는 것을 말한다.
   - 번갈아 가며 프로세스가 CPU를 할당받는 데 이때 `Context Switching`이 발생한다.
   - 사용자가 체감하기 힘든 속도로 `Context Switching`되며 프로세스가 처리되기 때문에 동시에 처리되는 것처럼 느껴진다.
2. **인터럽트 핸들링**
   - 인터럽트란 컴퓨터 시스템에서 예외 상황이 발생했을 때 CPU에게 알려 처리할 수 있도록 하는 것을 말한다.
   - 인터럽트가 발생하면 `Context Switching`이 발생한다.
   - `I/O request` : 입출력 요청
   - `time slice expired` : CPU 사용시간이 만료
   - `fork a child` : 자식 프로세스 생성
   - `wait for an interrupt` : 인터럽트 처리 대기
3. **사용자와 커널 모드 전환**
   - 사용자와 커널 모드 전환은 `Context Switching`이 필수는 아니지만 운영체제에 따라 발생할 수 있다.