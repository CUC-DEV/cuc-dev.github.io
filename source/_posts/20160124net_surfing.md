title: 科学上网流程介绍
date: 2016-01-24 09:30:43
tags: [tuto, task]
---
![科学上网](/img/net_surfing/surfing.jpg)
>科学上网有助于大家学习，在这里介绍设置流程，望大家合理利用

# 前期准备
首先你需要为电脑安装谷歌浏览器，然后下载简聊“分享”的两个文件：publickey.crt（证书）、SwitchyOmega.crx（谷歌浏览器的一个插件）。
# 配置过程
- 将证书（publickey.crt）添加信任 [参考教程](http://cnzhx.net/blog/self-signed-certificate-as-trusted-root-ca-in-windows/)
 - 双击publickey.crt文件
 - 点击安装证书
 - 选择将所有的证书放入下列存储，点击浏览
 - 选择受信任的根证书颁发机构，点击确定
  ![](/img/net_surfing/crt.jpg)
- 设置谷歌浏览器证书
 - 在“设置”中点击“显示高级设置”
 - 点击“管理证书”
  ![](/img/net_surfing/setting1.png)
 - 选择“受信任的根证书颁发机构”选项卡，点击“导入”，并选择publickey.crt文件所在路径
  ![](/img/net_surfing/setting2.png)
 - 导入成功后可以看到“neomedia.top”
  ![](/img/net_surfing/setting3.png)
- 为谷歌浏览器添加插件
 - 将SwitchyOmega.crx文件直接拖入扩展程序即可安装
  ![](/img/net_surfing/setting4.png)
- 设置SwitchyOmega
 - 点击上图中标注的红色位置“选项”
 - 点击左侧边栏中的proxy，按照图片中填写，点击“应用选项”
  ![](/img/net_surfing/setting5.png)
 - 浏览器上谷歌的官网，输入用户名和密码，地址栏右边会多一个圈圈，点击圈圈，鼠标悬停在“proxy”上会出现“HTTPS neomedia.top：4128”
  ![](/img/net_surfing/setting6.png) 
 - 在搜索栏搜索“where is my ip”可以看到如下
  ![](/img/net_surfing/setting7.png)
# 补充说明
此方法主要目的是方便大家查阅资料，不是很适合看视频，会很慢，当浏览过内网站的时候可以讲代理关闭，用户名和密码在简聊里找，希望大家合理利用~~~


