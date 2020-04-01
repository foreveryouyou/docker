### alpine
FROM alpine:latest

RUN apk add -U tzdata \
    && cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime \
    && apk del tzdata \
    && rm -rf /var/cache/apk/*
