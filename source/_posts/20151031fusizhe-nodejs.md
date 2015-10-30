title: 傅思喆nodejs学习总结
tags:
  - presentation
  - fusizhe
  - nodejs
type: presentation
date: 2015-10-31 01:15:04
---
{% raw %}
<section>
    <h1>NodeJS学习总结</h1>
    <p>
        <small>2015年10月31日</small>
    </p>
</section>

<section>
    <h2>NodeJS
    <p>Node简介</p>
    <p>代码逻辑</p>
    <p>模块<p>
    <p>事件流</p>
</section>

<section>
    <h2>Node简介</h2>
    <p><b>Node</b> 是一个服务器端 JavaScript 解释器</p>
    <p><b>目标</b>:帮助程序员构建高度可伸缩的应用程序</p>
    <p><b>优势</b>:运行Google V8 JavaScript引擎，所以速度和性能非常好</p>
</section>
   
<section>
    <section>
    <h2>代码逻辑</h2>
    <p>require('xxx')</p>
    <p>xxx.yyyyy</p>
    <p>xxx.listen()</p>
    </section>
   
    <section>
        <h3>require导入模块</h3>
        <p>全局方法require()是用来导入模块的，一般直接把 require() 方法的返回值赋值给一个变量，在 JavaScript 代码中直接使用此变量即可 。</p>
        <p>如加载http模块：require('http')</p>
    </section>

    <section>
        <h3>模块方法调用</h3>
        <p>根据不同模块和需求调用不同的模块方法实现最终效果</p>
        <p>例如创建服务：xxx.createServer 是'http'模块的方法，目的就是创建并返回一个新的web server对象，并且给服务绑定一个回调，用以处理请求。</p>
    </section>
  
    <section>
        <h3>添加监听</h3>
        <p>xxx.listen()方法可以让该模块对象在特定端口实现监听</p>
    </section>
    
    <section>
        <h4>通过以上对基础模块和方法的调用就可以实现一个最简单的页面了</h4>
    </section>
</section>

<section>
    <section>
    <h2>Node模块</h2>
    <p>模块使用</p>
    <p>模块开发</p>
    </section>
    
    <section>
        <h3>模块的使用</h3>
        <p>require('name')<br>——如果是系统预置的模块</p>
        <p>require('./.../xxx.js')<br>——加载制定目录下的模块</p>
    </section>
        
    <section>
        <h3>开发模块要点</h3>
        <p>模块内var定义的变量或方法为私有，不可直接调用，会出现undefind<p>
        <p>共有属性和方法定义需要用this.xxxx</p>
    </section>
</section>

<section>
    <h2>事件流</h2>
    <p>因为Node 采用的是事件驱动的模式，其中的很多模块都会产生各种不同的事件，可由模块来添加事件处理方法，所有能够产生事件的对象都是事件模块中的 EventEmitter 类的实例。</p>
</section>

<section>
    <h3>EventEmitter 类中的方法</h3>
    <p>addListener(event, listener) 和 on(event, listener) 都是将一个监听器添加到指定事件的监听器数组的末尾</p>
    <p>once(event, listener) 为添加一次性的监听器</p>
    <p>removeListener(event, listener) 将监听器从指定事件的监听器数组中移除</p>
    <p>emit(event, [arg1], [arg2], [...]) 方法用来产生事件</p>
</section>

<section>
    <h1>谢谢！</h1>
</section>


    
{% endraw %}