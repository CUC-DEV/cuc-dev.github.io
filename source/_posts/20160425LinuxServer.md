title: 运维笔记
date: 2016-04-25 16:33:16
tags: [LinuxServer,qiuzihe]
---
服务器重新启动后，有些服务需要手动开启，下面介绍一下需要手动开启的服务
#  一、启动gitblit
首先，在docker中显示所有的container，包括未运行的
### $ sudo docker ps -a
![docker](/img/linuxserver/docker.png)
上图所示中发现gitblit没有启动，于是手动启动gitblit
### $ sudo docker restart gitblit
![重启gitblit](/img/linuxserver/dockerrestart.png)
重启gitblit之后，重新显示所有的container
![重新显示container](/img/linuxserver/docker2.png)
上图的第一行证明启动gitblit成功
#  二、重启网站
每次重启了服务器之后进入实验室网址会出现下面内容，说明网站没有启动，下面就将一下如何启动网站。
![pm2查看进程](/img/linuxserver/webpage.png)
首先进入网站文件放置位置/opt/imc/site
### $cd /opt/imc/site
实验室网站进程利用pm2来进行管理。[pm2](https://github.com/Unitech/pm2) 是一个带有负载均衡功能的Node应用的进程管理器。
在site文件夹下，先查看一下目前运行的进程
### $pm2 ls
![pm2查看进程](/img/linuxserver/pm2ls0.png)
发现没有运行的进程。
### $pm2 start web.js --name site
![pm2启动网站](/img/linuxserver/pm2start.png)
启动之后再次查看运行的进程
### $pm2 ls
![pm2查看进程](/img/linuxserver/pm2ls.png)
发现现在实验室网站可以正常运行啦啦啦～～～
#  三、备注
如果网站运行出现其他问题导致运行异常，尝试用下列命令找到并解决问题。
### $ pm2 logs  # Display logs of all apps
### $ pm2 monit # Monitoring all processes launched:
### $ pm2 restart site # Restart app(site)
### $ sudo service apache2 reload  #restart apache
### $ sudo service apache2 start  #restart apache
