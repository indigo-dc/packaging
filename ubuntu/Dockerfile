FROM evarga/jenkins-slave
MAINTAINER Cristina Aiftimiei <cristina.aiftimiei@cnaf.infn.it>

USER root

RUN sed -i '/Defaults *requiretty/s/^/#/' /etc/sudoers
RUN sed -i '/root\tALL=/a jenkins ALL=(ALL) NOPASSWD: ALL' /etc/sudoers

RUN apt-get update
RUN apt-get -y install git maven cmake dpkg-dev devscripts debhelper
