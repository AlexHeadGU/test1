#build
FROM ubuntu:20.04
MAINTAINER headgus <alex-davydov211@mail.ru>

RUN apt-get update
RUN apt-get install tomcat9 -y

ENV CATALINA_HOME=/usr/share/tomcat9
ENV PATH $CATALINA_HOME/bin:$PATH
WORKDIR $CATALINA_HOME
RUN mkdir -p "$CATALINA_HOME"

CMD ["catalina.sh", "run"]
