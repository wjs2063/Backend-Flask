## http




### HTTP: 웹상에서 네트워크를 통해 서버사이에 통신할때 어떠한 형식으로 서로 통신하자고 규정해놓은 통신형식 혹은 통신구조라고 보면된다.이러한 통신형식을 프로토콜이라하고 그중하나가 HTTP이다

### HTTP 통신방식: 요청(request)과 응답(response)의 구조로 되어있다. HTTP를 기반으로 통신할때 client 가 server 에 HTTP요청을 보내면 server 는 처리후 client 에게 응답보냄

### FLASK 가 HTTP 부분을 자동으로 처리해주기때문에 개발자는 최대한 일반함수를 구현만하면 쉽게 엔드포인트 구현이 가능함


### STATELESS: 요청과 응답만이 존재하기때문에 진행상태등 관리하지않아도됨, BUT 보낼때마다 매번 다른데이터를 포함해서 요청을 보내야함 ( 이를해결하기위해 COOKIE 나 SESSION을 이용)

COOKIE : client측에서 data 저장
SESSION : server 측에서 data 저장
