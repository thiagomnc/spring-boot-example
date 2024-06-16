# spring-boot-example

## Guides
https://spring.io/guides/gs/spring-boot-docker

Gradle:
./gradlew build && java -jar build/libs/gs-spring-boot-docker-0.1.0.jar
docker build --build-arg JAR_FILE=build/libs/\*.jar -t springio/gs-spring-boot-docker .

Maven:
./mvnw package && java -jar target/demo-0.0.1-SNAPSHOT.jar
docker build -t springio/gs-spring-boot-docker . && docker run -p 8080:8080 springio/gs-spring-boot-docker
