# If you need to debug your application from within the container, you might consider temporarily
# switching this line to the following to pull a Ubuntu-based image instead of Alpine-based:
# FROM adoptopenjdk/openjdk11-openj9:latest
FROM adoptopenjdk/openjdk11-openj9:alpine-slim

ARG JAR_FILE=target/game.jar
COPY ${JAR_FILE} /srv/app.jar
ENTRYPOINT ["java","-jar","/srv/app.jar"]
