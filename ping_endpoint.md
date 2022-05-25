### 엔드포인트 : API 서버가 제공하는 통신채널 혹은 접점. 프론트엔드 서버등의 client 가 백엔드 API 서버와 통신할때 엔드포인트에 접속하는 형태로 통신
### 각 엔드포인트는 고유의 URL 주소를 가지게되고 URL 주소를 통해 엔드포인트에 접속


1. mkdir -p ~/Projects/api
2. cd ~/Projects/api
3.vim app.py

##--
from flask import Flask

app=Flask(__name__)

@app.route("/ping",methods=['GET'])
def ping():
        return "pong"
## ---


4.FLASK_APP=app.py FLASK_DEBUG=1 flask run : DEBUG 모드활성화: 코드수정되었을때 자동으로 재시작됨
5. brew install httpie

터미널 창 새로열고

http -v GET http://localhost:5000/ping

### pong 이 응답오는것을 알수있음




