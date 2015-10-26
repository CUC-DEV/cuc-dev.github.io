title: 第三次项目例会
tags:
  - presentation
type: presentation
date: 2015-10-25 10:07:49
---
{% raw %}
<section>
    <h1>新媒体项目会议</h1>
    <h3>第三次项目例会</h3>
    <p>
        <small>2015年10月25日</small>
    </p>
</section>
<section>
    <section>
        <h2>上周总结</h2>
    </section>
    <section>
        <h2>阿里云配置</h2>
        <ul>        
            <li>域名购买 neomedia.top</li>
            <li>安装jira: jira.neomedia.top</li>
            <li>安装jenkins: jenkins.neomedia.top</li>
            <li>通告网站: news.neomedia.top(暂有问题)</li>
            <li>实验室网站原型: lab.neomedia.top(欢迎乱点)</li>
            <li>实验室网站原型: dev.lab.neomedia.top(暂未开放)</li>
        </ul>
    </section>
    <section>
        <h2>Daily报告</h2>
        <p class="fragment">情况非常不错，大家继续保持</p>
    </section>
    <section>
        <h2>html学习</h2>
        <ul>
            <li class="fragment"><a href="https://code.google.com/p/zen-coding/wiki/ZenHTMLSelectorsEn">zen-coding</a></li>
        </ul>
    </section>
     <section>
        <h2>css学习</h2>
    </section>
    <section>
    <h2>jQuery学习</h2>
    </section>
</section>
<section data-background-transition="zoom" data-background="#4d7e65" data-transition="slide">
    <h2>运气大比拼<button class="fragment" id="whoIsLucky" style="width:50px;height:30px;color:red">人品</button></h2>
    <h4 id="who">组内学习</h2>
</section>
 <section>
        <h2>Jira的学习</h2>
        <ul>
            <li class="fragment">spint</li>
            <li class="fragment">task</li>
            <li class="fragment">subtask</li>
            <li class="fragment">tempo</li>
        </ul>
</section>
 <section>
        <h2>Hexo的学习</h2>
        <ul>
            <li class="fragment">模板post</li>
            <li class="fragment">模板ppt</li>
            <li class="fragment">branch：master + source</li>
            <li class="fragment">提交与发布</li>
        </ul>
</section>
 <section>
        <h2>关于分享环节的讨论</h2>
        <ul>
            <li class="fragment">每个人都做ppt，随机选择</li>
            <li class="fragment">每周提前制定</li>
            <li class="fragment">每人一部分，协同</li>
        </ul>
</section>
 <section>
        <h2>意见与建议</h2>
         <ul>
            <li class="fragment">分享文档</li>
        </ul>
</section>
<section>
    <h2><a href="/2015/10/17/20151025WeeklyPlanning/" target="_blank">下周任务</a>简介</h2>
</section>
<section>
    <h2>任何问题？</h2>
</section>
<script src="/libs/jquery-1.11.3.min.js" type="text/javascript"></script>
<script>
    var dice;
    var who;
    $(document).ready(function(){
        $("#whoIsLucky").click(whoIsLucky);
        $(document).keyup(function(evt) {
            if (evt.keyCode == 13) {
                if(dice){
                    clearInterval(dice);
                }
            }
        });
    });
    
    function whoIsLucky(){
        var members = ["曾䶮","仇紫荷","应泽峰","傅思喆"];
        dice = setInterval(function(){ 
            who = members[Math.floor(Math.random()*4)];
        $("#who").text(who+"分享学习心得");
        $("#whoIsLucky").off('click');
        }, 50);
    }
</script>
{% endraw %}