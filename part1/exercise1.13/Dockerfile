FROM openjdk:8

WORKDIR /usr/app

RUN git clone https://github.com/docker-hy/spring-example-project.git . && \
    ./mvnw package

EXPOSE 8080

CMD [ "java", "-jar", "./target/docker-example-1.1.3.jar" ]