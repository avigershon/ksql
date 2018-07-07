FROM ubuntu:16.04

RUN apt-get update

RUN apt-get install -y git

RUN apt-get install -y maven

RUN git clone https://github.com/confluentinc/ksql.git
RUN cd ksql

RUN mvn clean compile install -DskipTests
