# Docker Build Maven Stage
FROM eclipse-temurin:17-jdk-alpine
# Copy folder in docker
WORKDIR /opt/app
COPY ./ /opt/app
RUN mvn clean install -DskipTests
# Run spring boot in Docker
FROM openjdk:8-jdk-alpine
COPY --from=build /opt/app/target/*.jar hotelroomdetails.jar

ENTRYPOINT ["java","-jar","/hotelroomdetails.jar"]
