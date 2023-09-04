FROM ilegeul/debian:8-gnuarm-gcc-x11-v3
MAINTAINER Liviu Ionescu <ilg@livius.net>
WORKDIR /root

RUN echo "deb [trusted=yes] http://archive.debian.org/debian jessie main non-free contrib" > /etc/apt/sources.list
RUN echo 'deb-src [trusted=yes] http://archive.debian.org/debian/ jessie main non-free contrib'  >> /etc/apt/sources.list
RUN echo 'deb [trusted=yes] http://archive.debian.org/debian-security/ jessie/updates main non-free contrib'  >> /etc/apt/sources.list;

RUN \
apt-get -y update && \
apt-get -y install apt-utils && \
apt-get -y dist-upgrade --fix-broken

CMD ["/bin/bash"]
