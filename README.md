PHP�ļ������ϴ�,��������ϴ�
PHP�ļ������ϴ�,��������ϴ�

PHP����ģ������ϴ��ļ�

https://github.com/shangjinglong/CrossdomainFileUpload

������WAMP

1.�޸�C:\Windows\System32\drivers\etc\hosts�ļ�
���
127.0.0.8	www.upload1.cc
127.0.0.9	www.upload2.cc

2.�޸�Apache����httpd-vhosts.conf�ļ�
���

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

3.���ļ���uploadDemo1��uploadDemo2������������Ŀ¼

4.����Apache

5.����www.upload1.cc�ļ��ϴ���www.upload2.cc��