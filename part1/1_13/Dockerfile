FROM openjdk:8
WORKDIR /workdir
COPY . .
EXPOSE 8080
RUN ./mvnw package
CMD java -jar ./target/docker-example-1.1.3.jar