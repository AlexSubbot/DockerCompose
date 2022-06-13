FROM maven:3.8.5-jdk-8
RUN apt update
RUN apt install git -y

WORKDIR /tmp
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git
WORKDIR /boxfuse-sample-java-war-hello
RUN mvn package
