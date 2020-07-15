# PHP Dockerfile
Dockerfile for php & nginx. php 容器 和 nginx 容器，php-fpm 处理PHP代码，nginx 处理纯前端和静态资源，实现前后端分离。 php 容器中 安装有（bcmath, Core, ctype, curl, date, dom, fileinfo, filter, ftp, gd, hash, iconv, json, libxml, mbstring, mcrypt, mongodb, mysqlnd, openssl, pcre, PDO, pdo_mysql, pdo_sqlite, Phar, posix, readline, redis, Reflection, session, SimpleXML, soap, sockets, sodium, SPL, sqlite3, standard, swoole, tokenizer, xml, xmlreader, xmlwriter, xsl, zip, zlib）等常用扩展。
## 目录结构
![avatar](http://chuantu.xyz/t6/739/1594801404x-1224475230.png)
### Project 1
- [hub.docker.com](https://hub.docker.com/r/clownlee/nginx-php-fpm) 上的镜像 `docker pull clownlee/nginx-php-fpm`
- 直接 build Dockerfile 创建 nginx 和 php 在一个容器里。
- nginx 默认配置文件 `/nginx-php/init/pro.conf` 
- web 项目目录为容器内的 `/www/pro/public` 目录下(基于 laravel 和 thinkphp 框架入口目录设计)