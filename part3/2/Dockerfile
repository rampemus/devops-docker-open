FROM ubuntu:16.04

RUN apt-get update && apt-get install -y \
    rtmpdump wget ffmpeg python3-dev python3-setuptools \
    python3-pip python3-crypto python3-requests python3-lxml \
    php-cli php-curl php-xml php-bcmath && \
    pip3 install yle-dl && \
    apt-get purge -y --auto-remove python3-pip && \
    rm -rf /var/lib/apt/lists/*

WORKDIR /downloads

ENTRYPOINT ["yle-dl"]
