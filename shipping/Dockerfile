FROM maven:3.9.16
# create /app and set the directoy to /app
WORKDIR /app
COPY pom.xml .
COPY src ./src
RUN mvn clean package
RUN mv target/shipping-1.0.jar shipping.jar
# ExecStart=/bin/java -jar /app/shipping.jar
CMD ["java", "shipping.jar"]