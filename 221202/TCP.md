# TCP

메시지를 잘게 쪼개서 전송을 하고 손상되거나 손실된 패킷이 있다면 재요청을 한다

데이터조각 = 패킷

큰상태로 보내면 대역폭이너무 커서 다른 데이터 통신에 방해가 될 수 있다.
신뢰성 무결성 보장

## 3-WAY HANDSHAKE

가상의 통신로 확보하기 위해 사용
6비트로 이루어진 TCP헤더에서 코드비트 플래그를 잘 활용
URG ACK PSH RST SYN FIN
모두 초기값은 0

### 연결시작 3way HANDSHAKE

SYN - 1 보냄 Client -> Server
SYN + ACK 둘다 1 Server -> Client
ACK - 1 보냄 Client -> Server

### 연결종료 4way HANDSHAKE

FIN - 1 Client -> Server
ACK - 1 Server -> Client
FIN - 1 Server -> Client
ACK - 1 Client -> Server

---

# IP

어느곳으로 보내야할지 정함
패킷들이 효율적으로 최종목적지로 가도록함

# UDP

TCP보다 신뢰성이 떨어지지만 전송 속도가 일반적으로 빠른 프로토콜
영상 에 사용
