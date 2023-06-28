
FROM ubuntu:latest

RUN apt update

RUN apt upgrade -y

RUN apt install postfix telnet -y

COPY main.cf /etc/postfix 

#EXPOSE PORTS
EXPOSE 25/tcp
EXPOSE 587/tcp

#Start the Postfix Service
CMD ["/usr/sbin/postfix", "start-fg"]