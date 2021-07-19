FROM nginx:1.19.3-alpine

LABEL author="wangcaitao"
LABEL version="1.0.0"

RUN apk --no-cache add tzdata; \
    echo "Asia/Shanghai" > /etc/timezone; \
    ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime