#build
FROM ubuntu:16.04
MAINTAINER headgus <alex-davydov211@mail.ru>
RUN apt-get update
RUN apt install tomcat9 -y
ENV CATALINA_HOME=/usr/local/tomcat
#ADD maven_value:/home/maven/boxfuse-sample-java-war-hello/hello-1.0.war /var/lib/tomcat9/webapps/
RUN systemctl restart tomcat
WORKDIR $CATALINA_HOME
CMD ["catalina.sh","run"]