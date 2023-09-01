FROM openjdk:8u102-jre

COPY ./jar/* /usr/src/shirodemo-1.0-SNAPSHOT.jar

WORKDIR /usr/src

EXPOSE 8080 5005

CMD ["java", "-jar", "-agentlib:jdwp=transport=dt_socket,server=y,suspend=n,address=5005", "/usr/src/shirodemo-1.0-SNAPSHOT.jar"]