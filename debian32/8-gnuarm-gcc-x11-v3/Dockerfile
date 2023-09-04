FROM ilegeul/debian32:8-gnuarm-gcc-x11-v2
MAINTAINER Liviu Ionescu <ilg@livius.net>
ENTRYPOINT ["linux32"]
WORKDIR /root

RUN echo "deb [trusted=yes] http://archive.debian.org/debian jessie main non-free contrib" > /etc/apt/sources.list
RUN echo 'deb-src [trusted=yes] http://archive.debian.org/debian/ jessie main non-free contrib'  >> /etc/apt/sources.list
RUN echo 'deb [trusted=yes] http://archive.debian.org/debian-security/ jessie/updates main non-free contrib'  >> /etc/apt/sources.list;

RUN \
apt-get -y update && \
apt-get -y upgrade && \
apt-get -y install patchelf

CMD ["/bin/bash"] 
