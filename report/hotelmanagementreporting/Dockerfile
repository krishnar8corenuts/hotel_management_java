# Docker Build Maven Stage
FROM openjdk:8-jdk-alpine
VOLUME /tmp
ADD target/hotelbooking.jar hotelreports.jar

ENTRYPOINT ["java","-jar","/hotelreports.jar"]
