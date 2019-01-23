FROM wangcaitao/openjdk:8u191-jre-alpine

LABEL author="wangcaitao"
LABEL version="0.1.1"

RUN apk update; \
    apk add --no-cache; \
    cd /usr; \
    mkdir -p fescar-server/data; \
    wget https://github.com/alibaba/fescar/releases/download/v0.1.1/fescar-server-0.1.1.tar.gz; \
    tar -zxf fescar-server-0.1.1.tar.gz -C fescar-server/; \
    rm -rf fescar-server-0.1.1.tar.gz;

WORKDIR /usr/fescar-server/bin

EXPOSE 8091

CMD ["sh", "fescar-server.sh", "8091", "/usr/fescar-server/data/"]
