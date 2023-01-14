FROM ubuntu:18.04
RUN apt update && \
    apt -y upgrade && \
    apt -y install xvfb x11-utils x11vnc qemu wget curl nano
RUN curl -skLo gdown https://raw.githubusercontent.com/kmille36/GoogleDriveCurl/main/gdown && chmod +x gdown
RUN bash gdown Porteus-CINNAMON.qcow2 1-Easy8BrLr5tQ2r4pe9HcetCJ12QUOsy

COPY Porteus-CINNAMON.qcow2 /
COPY entrypoint.sh /
ENTRYPOINT ["/entrypoint.sh"]

