# 用PHP快速在你的Linux VPS上搭建网页服务器
在Windows下，你可以找到许多搭建服务器的简单软件，动动手指就可以下载。但是，在Linux下，这将会略复杂一点，毕竟并不是每个人都懂得Shell指令。那么，这个教程就在帮你解决此事。

## 登录服务器
首先，登录服务器是必要的。登录的方法因人而异，服务器的控制面板也会提供必要的帮助，但基本上都是SSH，这篇教程也是针对SSH的。如果服务器控制面板只给你了FTP链接，那么基本上就是把文件扔进去就好。

## 开始安装
登陆进去之后，简单执行一下下面这些命令中对应VPS所用系统的一条:

Ubuntu(20.04) :
```
apt install php -y 
```
Ubuntu(其他版本):
```
apt install php apache2 -y
```
Centos(未测试):
```
yum -y install php apache2
```
Archlinux(未测试) :
```
pacman -S php apache2 
```
如果不知道自己用的什么系统，就把上面的全执行一遍。

然后，这个应该是统一的:
```
service httpd start
```
## 测试
这个简单，访问一下你的服务器的IP。
