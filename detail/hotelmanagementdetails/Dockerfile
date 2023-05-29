# Docker Build Maven Stage
FROM openjdk:8-jdk-alpine
VOLUME /tmp
ADD target/hotelbooking.jar hoteldetails.jar

ENTRYPOINT ["java","-jar","/hoteldetails.jar"]
