FROM ubuntu:22.04

RUN apt update
RUN apt upgrade -y
RUN apt-get install xvfb x11-utils x11vnc qemu wget curl nano -y

RUN wget https://raw.githubusercontent.com/kmille36/GoogleDriveCurl/main/gdown
RUN bash gdown Porteus-CINNAMON.qcow2 1-Easy8BrLr5tQ2r4pe9HcetCJ12QUOsy

COPY Porteus-CINNAMON.qcow2 /
COPY entrypoint.sh /
ENTRYPOINT ["/entrypoint.sh"]

