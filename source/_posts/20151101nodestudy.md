title: 'nodejs学习总结应泽峰'
tags:
  - presentation
type: presentation
date: 2015-10-30 21:55:44
---
{% raw %}
<section>
    <h1>nodejs学习总结</h1>
</section>
<section>
  <h2>nodejs</h2>
  <section>
  <h3>什么是node?</h3>
  <li>Node是JavaScript语言的服务器运行环境。</li>
  <li class="fragment">提供大量工具库，使得JavaScript语言与操作系统互动</li>
  </section>
</section>

<section>
  <h2>搭建http服务器</h2>
<section>
  <h3>1.模块化</h3>
  <li>require()</li>
  <p>require命令用于指定加载模块，加载时可以省略脚本文件的后缀名</p>
  <p>模块可以是自己定义的也可以是其本身自带的功能模块</p>
  <p>如:http：提供HTTP服务器功能。</p>
</section>
<section>
  <h3>2,调用方法</h3>
  <li>http.createServer(function (request, response){}</li>
  <li>ceateServer方法接受一个函数作为参数，该函数的request参数是一个对象，表示客户端的HTTP请求</li>
  <li>response参数也是一个对象，表示服务器端的HTTP回应</li>
</section>
<section>
  <h4>3,通过 http.listen() 方法就可以让该 HTTP 服务器在特定端口监听。</h4>
</section>
<section>
  <h3>4,调用</h3>
  <li>用node调用这个文件，服务器就开始运行了。</li>
</section>
</section>
<section>
  <h3>express框架</h3>
  <li>目前最流行的基于Node.js的Web开发框架，可以快速地搭建一个完整功能的网站</li>
</section>
<section>
  <h3>express项目结构</h3>
  <li>app.js： 项目入口</li>
  <li>node_modules： 存放项目的依赖库</li>
  <li>package.json： 项目依赖配置及开发者信息</li>
  <li>routes： 路由文件</li>
  <li>Views： 页面文件</li>
</section>
<section>
  <h3>express方法</h3>
  <section>
  <li>app.listen()</li>
  <p>在给定的主机和端口上监听请求</p>
  <li> app.set(name, value)</li>
  <p>set()为设置 name 的值设为 value</p>
  </section>
  <section>
  <li>app.engine</li>
  <p>重新设置模板文件的扩展名</p>
  <li> app.use([path], function)</li>
  <p>使用中间件 function,</p>
  </section>
</section>
<section>
<h1>THANKS</h1>
</section>
{% endraw %}