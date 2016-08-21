FROM krodec/java8
MAINTAINER krodec <sergejmeister@web.de>

RUN mkdir -p /opt/intellijob
WORKDIR /opt/intellijob
WORKDIR /opt/intellijob/data
WORKDIR /opt/intellijob/mongoData
COPY intellijob.jar /opt/intellijob/
COPY data /opt/intellijob/data
COPY mongoData /opt/intellijob/mongoData

EXPOSE 8080

ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/opt/intellijob/intellijob.jar"]
