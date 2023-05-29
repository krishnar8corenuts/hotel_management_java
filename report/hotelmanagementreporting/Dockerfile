# Docker Build Maven Stage
FROM adoptopenjdk/openjdk11
VOLUME /tmp
ADD target/hotelbooking.jar hotelreports.jar

ENTRYPOINT ["java","-jar","/hotelreports.jar"]
