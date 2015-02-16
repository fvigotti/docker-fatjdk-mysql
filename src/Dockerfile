FROM fvigotti/docker-fatjdk8:latest

RUN apt-get -y update && \
    apt-get -y --quiet upgrade && \
    apt-get -y --quiet install libxml2-dev libxslt1-dev git python python-setuptools python-dev build-essential libz-dev lsb openssl dnsutils curl rsync iptraf-ng rdiff ethtool iotop libtool pv curl unzip zip inotify-tools && \
    apt-get -y --quiet install python-software-properties software-properties-common && \
    easy_install pip && \
    apt-get -y update && \
    apt-get -y clean


RUN echo oracle-java8-installer shared/accepted-oracle-license-v1-1 select true | sudo /usr/bin/debconf-set-selections

RUN add-apt-repository -y ppa:webupd8team/java && \
 apt-get update  -y && \
 apt-get install python-software-properties -y && \
 apt-get install software-properties-common -y && \
 add-apt-repository ppa:webupd8team/java -y && \
 apt-get update -y && \
 apt-get install oracle-java8-installer -y && \
 apt-get install oracle-java8-set-default -y



#WORKDIR /opt

#ENTRYPOINT ["java", "-jar", "/whatever/your.jar"]

