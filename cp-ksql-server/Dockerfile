FROM maven:alpine

RUN git clone https://github.com/confluentinc/ksql.git
RUN cd ksql

RUN mvn clean compile install -DskipTests
