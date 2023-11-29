FROM ubuntu:20.04

RUN apt-get update -y
RUN apt-get install coturn -y

EXPOSE 3478/tcp
EXPOSE 3478/udp

CMD  turnserver -v -r 10.0.0.36  -a -o -c /etc/turnserver.conf   & sleep infinity
