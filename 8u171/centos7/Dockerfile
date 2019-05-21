FROM centos:7

RUN yum install -y nano ca-certificates curl wget \
 && yum clean all

MAINTAINER Morten Andersen <moander@outlook.com>

RUN mkdir -p /usr/java \
 && curl -sS https://storage.googleapis.com/mpub/java/jdk-8u171-linux-x64.tar.gz \
  | tar -zxvC /usr/java

ENV JAVA_HOME=/usr/java/jdk1.8.0_171

ENV PATH=${JAVA_HOME}/bin:${PATH}

