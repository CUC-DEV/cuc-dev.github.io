title: JavaScript学习(仇紫荷)
tags:
- presentation
type: presentation
date: 2015-11-01 16:14:41
---
{% raw %}
<section>
    <h1>新媒体项目会议</h1>
    <h3>JavaScript学习总结</h3>
    <h6>仇紫荷</h6>
    <p>
        <small>2015年11月1日</small>
    </p>
</section>

<section>
    <section>
    <h3>JavaScript</h3>
    <p>JavaScript是由Netscape公司开发并随Navigator导航者一起发布的、介于Java与HTML之间、基于对象事件驱动的编程语言。正日益
    受到全球关注。因为他的开发环境简单，不需要Java编辑器，而是直接运行在Web浏览器中，因而备受Web设计者的所爱。
    </p>
    </section>
    <section>
        <h3>JavaScript</h3>
        <ul>
            <li>JavaScript被设计用来向HTML页面添加交互行为</li>
            <li>JavaScript是一种脚本语言（脚本语言是一种轻量级的编程）</li>
            <li>JavaScript是一种解释性语言（代码执行不进行预编译）</li>
        </ul>
    </section>
</section>

<section>
    <section>
        <h3>JavaScript和Java的区别</h3>
        <ul>
            <li>Java是SUN公司推出的新一代面向对象的程序设计语言，特别适合于Internet应用程序开发</li>
            <li>JavaScript是Netscape公司的产品，其目的是为了扩展Netscape Navigator功能，而开发的一种可以嵌入Web界面中的基于对象和事件驱动的解释性语言，它的前身是Live Script</li>
        </ul>
    </section>
    <section>
        <h3>JavaScript和Java的区别</h3>
        <ul>
            <li>Java是一种真正的面向对象的语言，即使是开发简单的程序，必须设计duxiang</li>
            <li>JavaScript是Netscape公司的产品，其目的是为了扩展Netscape Navigator功能，而开发的一种可以嵌入Web界面中的基于对象和事件驱动的解释性语言，它的前身是Live Script</li>
        </ul>
    </section>
</section>

<section>
    <section>
        <h3>JavaScript基本语法</h3>
        <ul>
            <li>HTML的  &#60;script &gt;标签用于把JavaScript插入HTML页面中</li>
            <img data-src="/img/JavaScript_study/10.jpg">
        </ul>
    </section>
    <section>
        <h3>基本数据类型</h3>
        <ul>
            <li>数值类型，比较常见的数据类型。在JavaScript语言中数值类型即可表示整数，也可以表示实数</li>
            <li>逻辑类型，主要用于逻辑计算，变量只有两个值，True和False</li>
            <li>字符串类型，由单引号或双引号包围的多个字符组成的</li>
            <li>未定义类型，又称为undefined类型，表示一个变量还没有赋予任何初值</li>
        </ul>
    </section>
    <section>
        <h3>运算符</h3>
        <ul>
            <li>赋值运算符：=,+=,-=,*=,/=,%=</li>
            <li>比较运算符：==,===(全等，包括值和类型),!=,>,<,>=,<=</li>
            <li>逻辑运算符：&&,||,!</li>
        </ul>
    </section>
    <section>
        <h3>用于字符串的‘+’运算符</h3>
        <ul>
            <li>txt1="Hello";</li>
            <li>txt2="world!";</li>
            <li>txt3=txt1+txt2;</li>
        </ul>
        <p>txt3="Hello world!"'</p>
    </section>
    <section>
        <h3>条件语句</h3>
        <ul>
            <li>if语句</li>
            <li>if...else语句</li>
            <li>if...else if...else语句</li>
            <li>switch语句</li>
        </ul>
    </section>
    <section>
        <h3>循环语句</h3>
        <ul>
            <li>for将一段代码循环指定的次数</li>
            <li>while当指定的条件为true是循环执行代码</li>
            <li>do...while循环是while循环的变种。该循环程序在初次运行时会首先执行一遍其中的代码，然后当之低昂的条件为true时它会继续这个循环</li>
        </ul>
    </section>
    <section>
        <h3>消息框</h3>
        <ul>
            <li>警告框 alert("文本")，当警告框出现后，用户需要点击确定按钮才能继续进行操作。</li>
            <li>确认框 confirm("文本")，当确认框出现后，用户需要点击确定或者取消按钮才能继续操作。如果用户点击确认，那么返回值为true。如果用户点击取消，那么返回值为false。</li>
            <li>提示框 prompt("文本","默认值")，当提示框出现后，用户需要输入某个值，然后点击确认或取消按钮才能继续操作。如果用户点击确认，那么返回值为输入的值。如果用户点击取消，那么返回值为pull。</li>
        </ul>
    </section>
    <section>
        <h3>JavaScript函数</h3>
        <p>函数是由事件驱动的或者当它被调用时执行的可重复使用的代码块</p>
        function 函数名（参数）{<br/>
        函数体;<br/>
        return 返回值;<br/>
        }<br/>
        <p>函数名对大小写是敏感的</p>
    </section>
</section>
<section>
    <section>
        <h3>基于对象的JavaScript语言</h3>
        <ul>
            <li>对象只是一种特殊的数据。对象拥有属性和方法。</li>
            <li>属性 指与对象有关的值。</li>
            <li>方法指对象可以执行的行为，或者可以完成的功能。</li>
        </ul>
    </section>
    <section>
        <h3>基于对象的JavaScript语言</h3>
        <p>JavaScirpt为编程人员提供了一些非常有用的采用内部对象和方法，例如String（字符串）、Math（数值计算）、Date（日期）等</p>
        <ul>
            <li>string对象的方法主要用于有关字符串在Web页面中的显示、字体大小、字体颜色、字符的搜索以及字符大小写转换。</li>
            <li>Date对象主要用于处理日期和时间。</li>
            <li>Math对象主要用于处理复杂的数学运算。</li>
        </ul>
    </section>
    <section>
        <h3>JavaScript事件</h3>
        <ul>
            <li>JavaScript使我们有能力创建动态页面。事件是可以被JavaScript侦测到的行为。</li>
            <li>网页中每个元素都可以产生某些触发JavaScript函数的事件。</li>
        </ul>
    </section>
    <section>
        <h3>JavaScript事件</h3>
        <ul>
            <li>JavaScript使我们有能力创建动态页面。事件是可以被JavaScript侦测到的行为。</li>
            <li>网页中每个元素都可以产生某些触发JavaScript函数的事件。</li>
        </ul>
    </section>
    <section>
        <h3>JEnd</h3>
    </section>
</section>


{% endraw %}





