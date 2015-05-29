FROM nimmis/java:openjdk-8-jre-headless

MAINTAINER max.scheffler@dius.com.au

RUN mkdir /custcollection

ADD *.jar /custcollection/

WORKDIR /custcollection

EXPOSE 8080

ENTRYPOINT ["/usr/bin/java", "-jar", "custcollection.api-1.0.jar"]
