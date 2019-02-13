FROM openjdk:8-jre-alpine

MAINTAINER  I2M Team @ HCC FU Berlin < i2m@zedat.fu-berlin.de>

RUN mkdir -p /opt/spotlight

ADD ../rest/target/rest-1.0-jar-with-dependencies.jar /opt/spotlight/dbpedia-spotlight.jar
COPY ../models/en /opt/spotlight/en
ADD spotlight.sh /bin/spotlight.sh
RUN chmod +x /bin/spotlight.sh

EXPOSE 8080