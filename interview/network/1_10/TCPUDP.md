# TCP와 UDP의 차이에 대해 설명해 주세요.

- 가장 큰 차이점은 **TCP는 연결 지향적 프로토콜, UDP는 비연결 지향적 프로토콜**이라는 것이다.
- `TCP`는 클라이언트와 **서버가 연결된 상태에서** 데이터를 주고 받고, `UDP`는 연결을 위해 **할당되는 논리적인 경로가 없고**, 각각의 패킷은 다른 경로로 전송되며, 독립적인 관계를 지닌다.
- `TCP`는 연속성보다 신뢰성 있는 전송이 중요할 때 사용되는 프로토콜이다.
- `UDP`는 TCP보다 빠르고 네트워크 부하가 적다는 장점이 있지만, 신뢰성 있는 데이터 전송을 보장하지는 않기 때문에 신뢰성보다는 연속성이 중요한 실시간 스트리밍과 같은 서비스에 자주 사용된다.

**TCP 특징**
1. 연결형 서비스로 가상 회선 방식을 제공
   - `3-way handshake` 과정을 통해 연결을 설정하고, `4-way handshake` 과정을 통해 연결을 해제한다.
2. 흐름 제어
   - 데이터 처리 속도를 조절하여 수신자의 버퍼 오버플로우를 방지한다.
3. 혼잡 제어
   - 네트워크 내의 패킷 수가 과도하게 증가하지 않도록 방지한다.
4. 높은 신뢰성 보장
   - 신뢰성이 높은 전송을 하기 때문에 UDP보다 속도가 느리다.
5. 전이중(Full-Duplex), 점재점(Point to Point) 방식
   - 전이중은 전송이 양방향으로 동시에 일어날 수 있고, 점재점은 각 연결이 정확히 2개의 종단점을 가지고 있다.

**UDP 특징**
1. 비연결형 서비스로 데이터그램 방식을 제공
   - 데이터의 전송 순서가 바뀔 수 있다.
2. 데이터 수신 여부를 확인하지 않는다.
   - TCP의 `3-way handshake` 같은 과정을 거치지 않는다.
3. 신뢰성이 낮다.
   - 흐름 제어가 없어서 제대로 전송되었는지, 오류가 없는지 확인할 수 없다.
4. TCP보다 속도가 빠르다.
5. `1:1`, `1:N`, `N:N` 통신이 가능하다.

[TCP, UDP](https://github.com/genesis12345678/TIL/blob/main/Http/network/network.md#tdp-udp)

|          | TCP        | UDP              |
|----------|------------|------------------|
| 연결 방식    | 연결형 서비스    | 비연결형 서비스         |
| 패킷 교환 방식 | 가상 회선 방식   | 데이터그램 방식         |
| 전송 순서    | 전송 순서 보장   | 전송 순서가 바뀔 수 있음   |
| 수신 여부 확인 | 수신 여부를 확인함 | 수신 여부를 확인하지 않음   |
| 통신 방식    | 1:1 통신     | 1:1, 1:N, N:N 통신 |
| 신뢰성      | 높다         | 낮다               |
| 속도       | 느리다        | 빠르다              |