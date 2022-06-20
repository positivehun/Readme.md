# 베이스이미지 버전
FROM node:16-alpine 

WORKDIR /app

COPY package.json package-lock.json ./
# npm ci 를 이용하면 버전에 맞는 패키지 설치
RUN npm ci

COPY index.js .

ENTRYPOINT [ "node","index.js" ]