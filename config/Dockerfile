FROM adoptopenjdk/openjdk11
COPY target/config-1V.jar /config.jar
COPY src/main/resources/application.properties /application.properties
ENV ENCRYPT_KEY=$ENCRYPT_KEY
ENTRYPOINT ["java","-Dspring.config.location=/application.properties","-jar","/config.jar"]