# Docker Build Maven Stage
FROM openjdk:8-jdk-alpine
VOLUME /tmp
ADD target/hotelbooking.jar hotelentities.jar

ENTRYPOINT ["java","-jar","/hotelentities.jar"]
