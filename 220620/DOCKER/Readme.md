# DOCKER 
https://www.youtube.com/watch?v=LXJhA3VWXFA 드림코딩 엘리 참고

## Node.js세팅
```
> npm init -y <-  node초기화(package.json설치)

>npm i express <-  Express설치

>node index.js <-  파일 실행
```



## localhost web제작하기(Node.js)
```
const express = require('express');

const app = express();

app.get('/', (req, res) => {
    res.send('POSITIVE X DOCKER');

});

app.listen(8080, () => console.log('Server is running'));
```

## dockerfile 만들기(Dockerfile)
```
# 베이스이미지 버전
FROM node:16-alpine 

WORKDIR /app

COPY package.json package-lock.json ./
# npm ci 를 이용하면 버전에 맞는 패키지 설치
RUN npm ci

COPY index.json .

ENTRYPOINT [ "node","index.js" ]
```


## docker빌드(Terminal)
```
docker build -f Dockerfile -t fun-docker . #마지막 점은 빌드 콘텍스트 현재 파일의 위치를 알려줌

docker images # 도커에 만들어진 이미지를 확인 가능하다

docker run -d -p 8080:8080 fun-docker # 도커 실행

docker ps # 현재 실행중인 이미지 확인

docker logs "컨테이너 아이디" # 현재 실행중인 컨테이너의 로그 확인 가능
```