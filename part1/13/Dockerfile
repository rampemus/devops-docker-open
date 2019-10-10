FROM java
WORKDIR /app
COPY . .
RUN java -version
RUN ./mvnw package
EXPOSE 8080
ENTRYPOINT ["java","-jar","./target/docker-example-1.1.3.jar"]
