FROM ubuntu:16.04
RUN apt-get update 
RUN apt-get upgrade -y
RUN apt-get install -y openssh-server supervisor
RUN mkdir -p /var/run/sshd
RUN mkdir -p /var/log/supervisor
COPY supervisord.conf /etc/supervisor/conf.d/supervisord.conf
EXPOSE 22 
CMD ["/usr/bin/supervisord"]

