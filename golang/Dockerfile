### golang
FROM golang:alpine

RUN apk add -U tzdata \
    && cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime \
    && apk del tzdata \
    && apk add -U git \
    && rm -rf /var/cache/apk/*
RUN go env -w GOPROXY=https://goproxy.cn,direct
