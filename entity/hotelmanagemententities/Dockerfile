# Docker Build Maven Stage
FROM openjdk:11
# Copy folder in docker
WORKDIR /opt/app
COPY ./ /opt/app
RUN mvn clean install -DskipTests
# Run spring boot in Docker
FROM openjdk:11
COPY --from=build /opt/app/target/*.jar hotelentities.jar

ENTRYPOINT ["java","-jar","/hotelentities.jar"]
