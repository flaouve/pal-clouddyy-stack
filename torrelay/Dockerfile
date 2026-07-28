FROM docker.io/library/debian:stable-slim

RUN apt update && \
apt install -y tor && \
rm -rf /var/lib/apt/lists/*

COPY torrc /etc/tor/torrc

ENTRYPOINT [ "tor", "-f", "/etc/tor/torrc" ]
