#build
FROM ubuntu:20.04
MAINTAINER headgus <alex-davydov211@mail.ru>
# Install modules
RUN apt update
RUN apt install -y default-jdk
RUN apt install -y maven
RUN apt install -y git


WORKDIR /home/maven/

RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git
WORKDIR boxfuse-sample-java-war-hello
RUN pwd
RUN mvn package
RUN ls

