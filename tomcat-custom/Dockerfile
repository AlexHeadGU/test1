#build
FROM tomcat:alpine
MAINTAINER headgus <alex-davydov211@mail.ru>
ENV CATALINA_HOME=/usr/local/tomcat
#ADD maven_value:/home/maven/boxfuse-sample-java-war-hello/hello-1.0.war /var/lib/tomcat9/webapps/
RUN systemd restart tomcat
WORKDIR $CATALINA_HOME
CMD ["catalina.sh","run"]