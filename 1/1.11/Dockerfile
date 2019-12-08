FROM node:10

RUN mkdir /app
WORKDIR /app

COPY backend-example-docker/ /app

RUN npm install

EXPOSE 8000

CMD npm start