# HTTP

Hyper Text Transfer Protocol

WWW -> 클릭으로 이동하기 시작함

---
# HTTP vs TCP

tcp/ip 프로토콜은 http와 어떻게 맞물려 동작하는 것일까?  그리고 무슨 차이가 있을까?

일단 가장 큰 차이점은 동작하는 계층이 다르다.

tcp/ip 는 transport 계층에서 동작한다. 

http는 application 계층에서 동작 한다. 이 계층에서 동작하는 프로토콜은 http  말고도 smtp, IMAP 등이 있다. 

개념적으로 살펴 보자면 HTTP, HTTPS, FTP 등의 프로토콜은 TCP/IP  이 위에서 동작하는 거라고 볼수ㅣ있다.

그중 http는 tcp/ip 위에서 어떤 형태로 웹에서 작동할지를 정해놓은  통신프로토콜일 뿐이다. 이 프로토콜위에서  http (하이퍼텍스트)를 전송 하는 규약)임.

그리고 http 통신은 비동기 통신을 기본으로하여 연결성 X

// 데이터 형태

tcp : byte array(binary)로 정보를 통신
http: String으로 정보를 통신

// 연결방식

tcp : 언제나 서버와 연결돼있어야하며, request 없이도 recevie가 일어남.
http: keep-alive로 지속적인 연결은 가능합니다만, 
기본적으론 close로 돼 있으며, request를 하여야만 recevie가 일어남


속도가 중요할땐? : 

tcp / IP 기반 소켓을 쓰는 것이 빠르다. 바인딩 과정 HTTP 변환 과정등이 생략되기 때문임.

연결지향 / 동기식 통신이 필요하다면 소켓 통신을 이용해야 한다.


[출처] tcp/ip와 http의 차이 |작성자 호떵