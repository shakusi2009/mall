FROM openjdk:8-jre-alpine

WORKDIR /app
COPY ./target/mall-admin-1.0-SNAPSHOT.jar /app

EXPOSE 8080
ENTRYPOINT ["sh", "-c"]
CMD ["java -Dcom.sun.management.jmxremote.port=19991 -Dcom.sun.management.jmxremote.authenticate=false -Dcom.sun.management.jmxremote.ssl=false -jar /app/mall-admin-1.0-SNAPSHOT.jar"]