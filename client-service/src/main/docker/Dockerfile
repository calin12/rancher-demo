FROM anapsix/alpine-java:8
EXPOSE 8900
COPY client-service.jar app.jar
RUN bash -c 'touch /app.jar'
ENTRYPOINT ["java","-server","-Xms128m","-Xmx256m","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]