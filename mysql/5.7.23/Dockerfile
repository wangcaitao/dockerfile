FROM mysql:5.7.23

LABEL author="wangcaitao"
LABEL version="1.0.0"

RUN echo "Asia/Shanghai" > /etc/timezone; \
    ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime; \
    dpkg-reconfigure -f noninteractive tzdata