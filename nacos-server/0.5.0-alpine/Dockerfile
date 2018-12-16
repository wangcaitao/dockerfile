FROM openjdk:8u151-jre-alpine

LABEL author="wangcaitao"
LABEL version="0.5.0"

RUN apk update; \
    apk add --no-cache; \
    cd /usr; \
    wget https://github.com/alibaba/nacos/releases/download/0.5.0/nacos-server-0.5.0.tar.gz; \
    tar -zxf nacos-server-0.5.0.tar.gz; \
    rm -rf nacos-server-0.5.0.tar.gz;

WORKDIR /usr/nacos/bin

EXPOSE 8848

CMD ["sh", "startup.sh", "-m", "standalone"]
