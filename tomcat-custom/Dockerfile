#build
FROM ubuntu:20.04
MAINTAINER headgus <alex-davydov211@mail.ru>

ENV CATALINA_HOME /usr/share/tomcat9

ENV PATH $CATALINA_HOME/bin:$PATH
WORKDIR $CATALINA_HOME
ENV CATALINA_BASE /var/lib/tomcat9
RUN apt-get update
RUN apt-get install tomcat9 -y
WORKDIR /home/maven/boxfuse-sample-java-war-hello
RUN pwd
ADD /target/hello-1.0.war /var/lib/tomcat9/webapps/hello-1.0.war
#RUN service tomcat9 restart
#EXPOSE 8080

CMD ["catalina.sh", "run"]
