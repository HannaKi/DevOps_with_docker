# Make sure you have java 8 installed
FROM amazoncorretto:22.0.0-alpine3.19

# Expose port
EXPOSE 8080

# Convention
WORKDIR /usr/src/app

# Copy all of the source code
COPY . .

# Build the project with ./mvnw package
RUN ./mvnw package

# Run with java -jar ./target/docker-example-1.1.3.jar
CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]

# The project should open in 8080 and you get a message by pressing the button.
