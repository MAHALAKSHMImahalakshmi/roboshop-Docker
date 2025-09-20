FROM maven
WORKDIR /opt/server
COPY pom.xml .
COPY src /opt/server/src 
# folder do not use src . it copy file so mention proper dir not current dir for storing dir
RUN mvn clean package
RUN mv /opt/server/target/shipping-1.0.jar /opt/server/shipping.jar
ENV CART_ENDPOINT="cart:8080" \
    DB_HOST="mysql"
    CMD ["java","-jar","shipping.jar"]