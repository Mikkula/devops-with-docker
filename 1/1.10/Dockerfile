FROM node:10

RUN mkdir /app
WORKDIR /app

COPY frontend-example-docker/ /app

RUN npm install

EXPOSE 5000

CMD ["npm", "start"]
