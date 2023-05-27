# Docker Build Maven Stage
FROM eclipse-temurin:17-jdk-alpine
# Copy folder in docker
WORKDIR /opt/app
COPY ./ /opt/app
RUN mvn clean install -DskipTests
# Run spring boot in Docker
FROM eclipse-temurin:17-jdk-alpine
COPY --from=build /opt/app/target/*.jar hotelentities.jar
 
ENTRYPOINT ["java","-jar","/hotelentities.jar"]


FROM adoptopenjdk/openjdk11:alpine-jre

ARG APP_NAME="hotelentities"
ARG APP_VERSION="0.0.1"
ARG JAR_FILE="/build/libs/${APP_NAME}-${APP_VERSION}.jar"

COPY ${JAR_FILE} hotelentities.jar
ENTRYPOINT ["java","-jar", "hotelentities.jar"]
