FROM maven:alpine

RUN apt-get update

RUN apt-get install -y git

RUN git clone https://github.com/confluentinc/ksql.git
RUN cd ksql

RUN mvn clean compile install -DskipTests
