FROM openjdk:8u191-jre-alpine

LABEL author="wangcaitao"
LABEL version="8u191-jre-alpine"

RUN apk --no-cache add tzdata; \
    ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime; \
    echo "Asia/Shanghai" > /etc/timezone