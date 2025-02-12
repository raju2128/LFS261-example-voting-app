FROM maven:3.9.8-sapmachine-21
WORKDIR /opt/app 
COPY . .
RUN mv target/worker-jar-with-dependencies.jar /run/worker.jar && \
    rm -rf /opt/app/*       
CMD ["java", "-jar", "/run/worker.jar"]
