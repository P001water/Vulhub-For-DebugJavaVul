FROM openjdk:8u102-jre

COPY ./jar/* /usr/src/fastjsondemo.jar
WORKDIR /usr/src
EXPOSE 8090 5005

CMD [ "java", "-Dserver.address=0.0.0.0", "-Dserver.port=8090", "-jar", "-agentlib:jdwp=transport=dt_socket,server=y,suspend=n,address=5005", "/usr/src/fastjsondemo.jar" ]