#build
FROM maven

RUN apt-get update
RUN apt-get install git
WORKDIR /usr/src/app
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git
RUN mvn package