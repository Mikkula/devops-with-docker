FROM node:10

RUN mkdir /app
WORKDIR /app

COPY frontend-example-docker/ /app

RUN npm install
RUN npm install -g serve
RUN npm run build

EXPOSE 5000

CMD serve -s -l 5000 dist/