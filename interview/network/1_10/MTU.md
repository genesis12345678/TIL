# MTU가 무엇인가요?

- Maximum Transmission Unit의 약자로, **최대 전송 단위**를 뜻한다.
- 데이터링크 에서 하나의 프레임 또는 패킷에 담아 운반 가능한 최대 크기
- `MTU`란 TCP/IP 네트워크 등과 같은 패킷 또는 프레임 기반의 네트워크에서 전송될 수 있는 최대 크기의 패킷 또는 프레임을 말한다.
- 한 번에 전송할 수 있는 최대 전송량(Byte)인 MTU 값은 매체에 따라 달라진다.
- 예를 들면 Ethernet 환경에라면 MTU 기본값은 1500, FDDI인 경우 4000, X.25는 576, Gigabit MTU는 9000 정도 등 매체 특성에 따라 한 번에 전송량이 결정된다.
- **상위 계층의 데이터의 수용 가능한 최대 크기로도 생각할 수 있다.**
- 따라서 상위 계층 프로토콜(네트워크 계층 이상)은 하위 계층인 데이터링크에서의 MTU에 맞추어야 한다. 그래서 IP 단편화 등을 시행할 수밖에 없다.

사실상 TCP 상에서 전송할 수 있는 사용자 데이터 최대 크기는 `MSS(Maximum Segment Size)`로, 기본적으로 설정된 MUT 값에 의해 결정된다.

예를 들어, Ethernet일 경우 MTU 1500에 IP 헤더크기 20byte, TCP 헤더크기 20byte를 제외한 1460이 MSS 값이다.

MSS = MTU - IP 헤더크기(최소 20byte) - TCP 헤더크기(최소 20byte)