FROM ubuntu:20.04
RUN apt-get update && \
    apt-get -y upgrade && \
    apt-get -y install xvfb x11-utils x11vnc qemu wget curl nano
RUN curl -skLo gdown https://raw.githubusercontent.com/kmille36/GoogleDriveCurl/main/gdown && chmod +x gdown && bash gdown Porteus-CINNAMON.qcow2 1-Easy8BrLr5tQ2r4pe9HcetCJ12QUOsy

COPY Porteus-CINNAMON.qcow2 /
COPY entrypoint.sh /
ENTRYPOINT ["/entrypoint.sh"]

