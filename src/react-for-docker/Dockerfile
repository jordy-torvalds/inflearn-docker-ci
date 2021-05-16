# 사용 백그라운드 이미지
FROM node:alpine

# 작업 폴더 이동 / -> /usr/src/app
WORKDIR /usr/src/app

# package.json을 /usr/src/app으로 복사
# 의존성 관리 json에 변경이 발생한 경우만 라이브러리 파일을 받도록 하기 위해 우선적으로 소스코드 표시
COPY package.json ./

RUN npm install

COPY ./ ./

CMD ["npm","run","start"]


