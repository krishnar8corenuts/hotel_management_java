# Docker Build Maven Stage
FROM adoptopenjdk/openjdk11
VOLUME /tmp
ADD target/hotelbooking.jar hotelroomdetails.jar

ENTRYPOINT ["java","-jar","/hotelroomdetails.jar"]
