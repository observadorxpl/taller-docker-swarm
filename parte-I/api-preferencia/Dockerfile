FROM openjdk:8-jdk-alpine
LABEL maintainer="w.marchanaranda@gmail.com"
WORKDIR /workspace
ADD target/api*.jar app.jar

ENV url_apipersona="apipersona"
ENV port_apipersona="8080"
ENV host="mysql_server"
ENV port="3306"
ENV database="demobd"
ENV username="root"
ENV password="toor"

ENTRYPOINT exec java -Djava.security.egd=file:/dev/./urandom -jar /workspace/app.jar
EXPOSE 8080