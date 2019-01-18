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

## openjdk

### 8u191-jre-alpine

* 其他 java 环境依赖 `FROM wangcaitao/openjdk:8u191-jre-alpine`

## mysql

### 5.7.23

* run 运行前先修改 `password` 为自己设置的密码  
  `# docker run -d -p 3306:3306 -p 33060:33060 --name mysql -v mysql:/var/lib/mysql -v mysql-conf:/etc/mysql -e MYSQL_ROOT_PASSWORD=password wangcaitao/mysql:5.7.23`