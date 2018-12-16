FROM alpine:3.7

LABEL author="wangcaitao"
LABEL version="1.0.0"

RUN apk update; \
    apk add --no-cache; \
    apk add tzdata; \
    ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime; \
    echo "Asia/Shanghai" > /etc/timezone; \
    apk add git; \
    apk add nodejs-npm; \
    npm install -g hexo-cli; \
    mkdir /usr/hexo; \
    hexo init /usr/hexo; \
    cd /usr/hexo; \
    npm install; \
    npm install hexo-deployer-git --save; \
    npm install hexo-generator-searchdb --save; \
    rm /var/cache/apk/*;

WORKDIR /usr/hexo

EXPOSE 4000

CMD ["hexo", "server"]
