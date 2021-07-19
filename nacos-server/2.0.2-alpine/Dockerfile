FROM wangcaitao/openjdk:8u191-jre-alpine

LABEL author="wangcaitao"
LABEL version="2.0.2"

RUN apk update; \
    apk add --no-cache; \
    cd /usr; \
    wget https://github.com/alibaba/nacos/releases/download/2.0.2/nacos-server-2.0.2.tar.gz; \
    tar -zxf nacos-server-2.0.2.tar.gz; \
    rm -rf nacos-server-2.0.2.tar.gz;

WORKDIR /usr/nacos/bin

EXPOSE 8848

CMD ["sh", "startup.sh", "-m", "standalone"]
