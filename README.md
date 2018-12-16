# dockerfile

记录 Dockerfile 以及运行命令

## nacos-server

### v0.5.0-alpine

* run standalone  
  `# docker run -d --name nacos-server -p 8848:8848 -v nacos-server:/usr/nacos wangcaitao/nacos-server:0.5.0-alpine`

## hexo

### 1.0.0-alpine

* run  
  `# docker run -d --name hexo -p 4000:4000 -v hexo:/usr/hexo wangcaitao/hexo:1.0.0-alpine`
* config hexo  
  [详细配置文档](http://wangcaitao.cn/hexo/docker/start/)