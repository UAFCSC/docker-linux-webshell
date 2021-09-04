FROM ubuntu:focal

RUN apt update && apt install -y openssh-server openssh-client
RUN mkdir /var/run/sshd

RUN echo 'root:csc' |chpasswd
RUN sed -ri 's/^#?PermitRootLogin\s+.*/PermitRootLogin yes/' /etc/ssh/sshd_config
RUN sed -ri 's/UsePAM yes/#UsePAM yes/g' /etc/ssh/sshd_config

RUN yes | unminimize

RUN mkdir /root/.ssh
CMD ["/usr/sbin/sshd", "-D"]