# Docker Build Maven Stage
FROM openjdk:8-jdk-alpine
VOLUME /tmp
ADD target/hotelbooking.jar hotelroomdetails.jar

ENTRYPOINT ["java","-jar","/hotelroomdetails.jar"]
