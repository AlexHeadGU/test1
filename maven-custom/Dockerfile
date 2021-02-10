#build
FROM maven
MAINTAINER headgus <alex-davydov211@mail.ru>
# Install modules
RUN apk update
RUN apk install -y \
		default-jdk \
		maven \
		git \


WORKDIR /home/maven/

RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git
WORKDIR boxfuse-sample-java-war-hello
RUN mvn package