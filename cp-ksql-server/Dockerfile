FROM ubuntu:16.04

RUN git clone https://github.com/confluentinc/ksql.git
RUN cd ksql

mvn clean compile install -DskipTests
