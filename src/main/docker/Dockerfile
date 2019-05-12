FROM openjdk:8u212-jdk-slim-stretch

ARG TARGET_DIR
ARG JAR_NAME

ENV TARGET_DIR $TARGET_DIR
ENV JAR_NAME $JAR_NAME

#PORT FORWARD
EXPOSE 8080

#INSTALLING APP
VOLUME /tmp
ADD ${TARGET_DIR}/${JAR_NAME} app.jar
RUN sh -c 'touch /app.jar'
ENV JAVA_OPTS=""
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /app.jar" ]