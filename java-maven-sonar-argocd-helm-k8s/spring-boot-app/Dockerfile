# Use Eclipse Temurin JDK 17 slim as runtime
FROM eclipse-temurin:17-jdk-jammy

# Artifact path from Maven build
ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app

COPY ${artifact} app.jar

# Run the Spring Boot app
ENTRYPOINT ["java", "-jar", "app.jar"]
