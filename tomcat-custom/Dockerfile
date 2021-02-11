#build
FROM ubuntu:20.04
MAINTAINER headgus <alex-davydov211@mail.ru>
RUN apt-get update
RUN apt-get install tomcat9 -y
ENV CATALINA_HOME /usr/share/tomcat9
ENV PATH $CATALINA_HOME/bin:$PATH
WORKDIR /home/maven/boxfuse-sample-java-war-hello
#ADD ./target/hello-1.0.war /var/lib/tomcat9/webapps/hello-1.0.war
RUN pwd
#RUN service tomcat9 restart
WORKDIR $CATALINA_HOME
CMD ["catalina.sh", "run"]