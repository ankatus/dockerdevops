FROM openjdk
WORKDIR /workdir
ADD spring-example-project-master ./
RUN ./mvnw package
CMD java -jar ./target/docker-example-1.1.3.jar