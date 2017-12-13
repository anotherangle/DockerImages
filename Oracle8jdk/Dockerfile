FROM ubuntu

MAINTAINER chetan.talwar@gmail.com

RUN \
  apt-get update && \
  apt-get install -y default-jre && \
  apt-get install -y default-jdk && \
  apt-get install -y software-properties-common && \
  add-apt-repository -y ppa:webupd8team/java && \
  apt-get update && \
  echo debconf shared/accepted-oracle-license-v1-1 select true | debconf-set-selections && \
  echo debconf shared/accepted-oracle-license-v1-1 seen true | debconf-set-selections && \
  apt-get install -y oracle-java8-installer && \
  apt-get update && apt-get install net-tools

