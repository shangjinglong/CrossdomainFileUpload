PHP文件跨域上传,跨服务器上传
PHP文件跨域上传,跨服务器上传

PHP本地模拟跨域上传文件

https://github.com/shangjinglong/CrossdomainFileUpload

环境：WAMP

1.修改C:\Windows\System32\drivers\etc\hosts文件
添加
127.0.0.8	www.upload1.cc
127.0.0.9	www.upload2.cc

2.修改Apache配置httpd-vhosts.conf文件
添加

#ServerAdmin webmaster@dummy-host.kekezu.com
DocumentRoot "E:/www_root/uploadDemo1"
ServerName www.upload1.cc
ErrorLog "logs/error.log"
CustomLog "logs/access.log" common
DirectoryIndex index.html index.htm index.php


#ServerAdmin webmaster@dummy-host.kekezu.com
DocumentRoot "E:/www_root/uploadDemo2"
ServerName www.upload2.cc
ErrorLog "logs/error.log"
CustomLog "logs/access.log" common
DirectoryIndex index.html index.htm index.php

3.将文件夹uploadDemo1，uploadDemo2拷贝到环境根目录

4.重启Apache

5.运行www.upload1.cc文件上传到www.upload2.cc下