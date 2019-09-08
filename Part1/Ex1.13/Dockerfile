FROM openjdk:8

WORKDIR /usr/springapp
COPY . .

RUN apt-get update
RUN ["./mvnw", "package"]
CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]