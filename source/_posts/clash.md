---
title: clash
date: 2021-10-27 16:46:14
tags:
---

#### clash 安装与使用
##### 项目地址:  *[clash](https://github.com/Dreamacro/clash/releases)*
##### arch 安装 sudo pacman -S clash 
##### 其它linux: 下载对应系统架构的压缩文件,如: clash-linux-amd64-v1.7.1.gz;也可下直接命令下载 
```shell 
wget -c https://github.com/Dreamacro/clash/releases/download/v1.7.1/clash-linux-amd64-v1.7.1.gz
```
##### 下载后执行以下命令
```shell
# 解压文件并不删除原文件
gunzip -c clash-linux-amd64-v1.7.1.gz > clash
# 给二进制文件添加执行权限
chmod +x clash
# 可以把clash移动到/usr/local/bin/下便于直接启动
cp chmod /usr/local/bin/
# 运行clash会在用户配置目录(.config/clash/)下生成配置文件
clash 
# 生成配置文件就可以停止clash 服务了(ctrl + c)
# 移动到clash配置目录
cd ~/.config/clash/
wget -O config.yaml  wget -O config.yaml https://subcon.dlj.tf/sub\?target\=clashr\&new_name\=true\&url\=https%3A%2F%2Fraw.fastgit.org%2Ffreefq%2Ffree%2Fmaster%2Fv2\&insert\=false\&config\=https%3A%2F%2Fraw.githubusercontent.com%2FACL4SSR%2FACL4SSR%2Fmaster%2FClash%2Fconfig%2FACL4SSR_Online.ini
# 命令后面跟的网址是机场的订阅网址,我是白嫖的,网站地址是[NV资源网](https://noisevip.cn/5911.html/),复制下方的订阅地址替换即可
# 再次执行clash,可以看到添加的订阅地址了
clash 
# 之后设置自己的浏览器代理
> http 127.0.0.1:7890
> sock5 127.0.0.1:7891
# 到此clash配置启动就完成了
```

##### linux 终端代理
```shell 
# arch安装proxychains-ng
sudo pacman -S proxychains-ng
# centos安装proxychains-ng
yum install proxychains-ng
# 安装完成后修改下配置文件
sudo nvim /etc/proxychains.conf
# 将结尾的sock代理改为sock5 127.0.0.1 7891
# 修改完后保存就可以直接使用了,eg: proxychains <command>;
proxychains git clone https://github.com/Dreamacro/clash.git



