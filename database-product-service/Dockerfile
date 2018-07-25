FROM java:8
EXPOSE 9000
RUN mvn clean install
ADD /target/database-product-service-0.0.1-SNAPSHOT.jar database-product-service-0.0.1-SNAPSHOT.jar
ENTRYPOINT [“java”,”-jar”,”database-product-service-0.0.1-SNAPSHOT.jar”]
