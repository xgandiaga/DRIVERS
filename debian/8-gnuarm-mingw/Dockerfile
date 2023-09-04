FROM ilegeul/debian:8-gnuarm-mingw-v2
MAINTAINER Liviu Ionescu <ilg@livius.net>
WORKDIR /root

RUN echo "deb [trusted=yes] http://archive.debian.org/debian jessie main non-free contrib" > /etc/apt/sources.list
RUN echo 'deb-src [trusted=yes] http://archive.debian.org/debian/ jessie main non-free contrib'  >> /etc/apt/sources.list
RUN echo 'deb [trusted=yes] http://archive.debian.org/debian-security/ jessie/updates main non-free contrib'  >> /etc/apt/sources.list;
RUN apt-get update

RUN \
apt-get -y install zip

CMD ["/bin/bash"]