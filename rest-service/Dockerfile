FROM amazoncorretto:11
COPY .mvn /.mvn
COPY src /src
WORKDIR ./
RUN ./mvnw install
RUN cp .db.json /target/
WORKDIR /target
CMD ["java", "-jar", "rest-service-0.0.1-SNAPSHOT.jar", "--server.port=${PORT}"]
