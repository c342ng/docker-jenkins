FROM golang:1.7.4
RUN apt-get update
RUN apt-get install -y openssh-server
RUN useradd -m -d /home/jenkins -s /bin/sh jenkins && echo "jenkins:jenkins" | chpasswd
EXPOSE 22
CMD ['/usr/sbin/sshd','-D']