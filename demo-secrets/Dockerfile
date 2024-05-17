# Use an official OpenJDK runtime as a parent image
FROM openjdk:11-jre-slim

# Set the working directory in the container
WORKDIR /app

# Copy the application JAR file
COPY target/demo-0.0.1-SNAPSHOT.jar app.jar

# Define the entry point for the container
ENTRYPOINT ["sh", "-c", "java -Dmyparam=${MY_SECRET_PARAM} -jar app.jar"]
