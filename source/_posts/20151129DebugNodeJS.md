title: NodeJS调试方法
date: 2015-11-29 14:13:43
tags: [tuto]
---
![NodeJS](/img/20151129_nodejs-logo.png)
>妈妈再也不同担心的我的调试了

# 前言
你想像调试前端js一样debug NodeJS程序吗?
# 安装工具
- 安装google chrome最新版
- 安装inspector工具：`npm install node-inspector -g`
- debug模式运行程序：`node --debug web.js`
- 新开terminal运行`node-inspector`连接nodejs程序,出现图片所示信息![inspector](/img/20151129_inspector.png)
- 在chrome浏览器中打开terminal显示的地址*http://127.0.0.1:8080/?ws=127.0.0.1:8080&port=5858 to start debugging*
- 稍等片以便加载后台所有源代码,如图![debug](/img/20151129_debug.png)
- 像前端一样调试js吧!
 
# 其他链接
- [google chrome调试教程](https://developer.chrome.com/devtools/docs/javascript-debugging)