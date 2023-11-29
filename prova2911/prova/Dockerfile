FROM eclipse-temurin:17-jdk-alpine

WORKDIR /app

COPY . /app

EXPOSE 8081

CMD ["./mvnw", "spring-boot:run"]

## docker build . -t daniloufla/app-spring:1.0.0
## docker run -p 8081:8081 daniloufla/app-spring:1.0.0
## docker login
## docker push daniloufla/app-spring:1.0.0
