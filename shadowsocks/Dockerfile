FROM exidakeng/alpine:latest

ADD shadowsocks-server.tar.gz /app/
WORKDIR /app

ENTRYPOINT ["/bin/bash", "-c", "/app/shadowsocks-server"]
