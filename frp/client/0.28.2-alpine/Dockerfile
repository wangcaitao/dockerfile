FROM alpine:3.7

LABEL author="wangcaitao"
LABEL version="0.28.2"

RUN apk update && \
    apk add --no-cache && \
    wget https://github.com/fatedier/frp/releases/download/v0.28.2/frp_0.28.2_linux_amd64.tar.gz && \
    tar -zxf frp_0.28.2_linux_amd64.tar.gz -C /usr/ && \
    rm -rf frp_0.28.2_linux_amd64.tar.gz && \
    cd /usr && \
    mv frp_0.28.2_linux_amd64 frp-client && \
    rm -rf frp-client/frps*

WORKDIR /usr/frp-client

CMD ["./frpc", "-c", "./frpc.ini"]
