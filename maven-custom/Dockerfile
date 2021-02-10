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
RUN mvn package

#build
FROM tomcat:alpine
MAINTAINER headgus <alex-davydov211@mail.ru>
ENV CATALINA_HOME=/usr/local/tomcat
ADD maven:/home/maven/boxfuse-sample-java-war-hello/hello-1.0.war /var/lib/tomcat9/webapps/
RUN systemctl restart tomcat
WORKDIR $CATALINA_HOME
CMD ["catalina.sh","run"]