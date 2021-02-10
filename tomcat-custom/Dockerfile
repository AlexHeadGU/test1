#build
FROM ubuntu:20.04
MAINTAINER headgus <alex-davydov211@mail.ru>
RUN apt-get update
RUN apt-get install tomcat9 -y
ENV CATALINA_HOME=/usr/local/tomcat
#ADD maven_value:/home/maven/boxfuse-sample-java-war-hello/hello-1.0.war /var/lib/tomcat9/webapps/
#RUN service restart tomcat9
WORKDIR $CATALINA_HOME
CMD ["catalina.sh","run"]