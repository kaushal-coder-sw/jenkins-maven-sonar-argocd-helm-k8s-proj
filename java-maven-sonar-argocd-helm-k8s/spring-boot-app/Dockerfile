# Use supported Java 17 base image
FROM eclipse-temurin:17-jre-alpine

# Jar artifact location
ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app

# Copy the jar built by Maven
COPY ${artifact} app.jar

# Run the Spring Boot app
ENTRYPOINT ["java","-jar","app.jar"]
