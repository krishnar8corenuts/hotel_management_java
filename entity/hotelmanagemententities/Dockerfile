# Docker Build Maven Stage
FROM adoptopenjdk/openjdk11
VOLUME /tmp
ADD target/hotelbooking.jar hotelentities.jar

ENTRYPOINT ["java","-jar","/hotelentities.jar"]
