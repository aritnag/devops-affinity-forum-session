# Start with a base image containing Java runtime
FROM openjdk:8-jdk-alpine
 
# Add Maintainer Info
LABEL maintainer="aritnag@deloitte.com"

# Add a volume pointing to /tmp
VOLUME /tmp
 
# Make port 8080 available to the world outside this container
EXPOSE 8888
 
# The application's jar file
ARG JAR_FILE=target/email-as-a-service-0.0.1-SNAPSHOT.jar
 
# Add the application's jar to the container
ADD ${JAR_FILE} email-as-a-service-0.0.1-SNAPSHOT.jar
 
# Run the jar file
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/email-as-a-service-0.0.1-SNAPSHOT.jar"]

