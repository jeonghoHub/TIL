URI와 웹 브라우저 요청 흐름

URI는 로케이터, 이름 또는 둘다 추가로 분류될 수 있다.

URI 단어 뜻

Uniform: 리소스 식별하는 통일된 방식
Resource: 자원, URI로 식별할 수 있는 모든 것(제한 없음)
Identifier: 다른 항목과 구분하는데 필요한 정보

URL - Locator: 리소스가 있는 위치를 지정
URN - Name: 리소스에 이름을 부여
위치는 변할 수 있지만, 이름은 변하지 않는다.

주소창에 www.google.com:443/search?q=hello&hl=ko 입력시

DNS조회 IP:200.200.200.2

1. 웹 브라우저가 HTTP 메세지 생성
GET /search?q=hello&hl=ko HTTP/1.1
Host:www.google.com

2. SOCKET 라이브러리를 통해 전달
	- A: TCP/IP 연결(IP, PORT)
	- B: 데이터 전달
3. TCP/IP 패킷 생성, HTTP 메시지 포함
