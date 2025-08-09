# You can change this base image to anything else
# But make sure to use the correct version of Java
FROM maven:3.8.7-openjdk-17

# Simply the artifact path
ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app

COPY ${artifact} app.jar

# This should not be changed
ENTRYPOINT ["java","-jar","app.jar"]
