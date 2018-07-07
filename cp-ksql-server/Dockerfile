FROM ubuntu:16.04

# Install OpenJDK-8
RUN apt-get update && \
    apt-get install -y openjdk-8-jdk && \
    apt-get install -y ant && \
    apt-get clean;

# Fix certificate issues
RUN apt-get update && \
    apt-get install ca-certificates-java && \
    apt-get clean && \
    update-ca-certificates -f;

RUN apt-get install -y git

RUN apt-get install -y maven

RUN git clone https://github.com/confluentinc/ksql.git
RUN cd ksql/cp-ksql-server

RUN mvn package -X -DskipTests
