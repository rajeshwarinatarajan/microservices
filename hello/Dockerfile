FROM openjdk:8-jdk-alpine
VOLUME /tmp
#ARG is available at build time only
#ARG JAR_FILE
COPY hello.jar app.jar
#EXPOSE <port>
RUN echo "Arg value set is ${JAR_FILE}"
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]

