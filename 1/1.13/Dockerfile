FROM openjdk:8

RUN mkdir /app
WORKDIR /app

COPY spring-example-project/ ./

RUN ./mvnw package

CMD ["java", "-jar", "target/docker-example-1.1.3.jar"]
