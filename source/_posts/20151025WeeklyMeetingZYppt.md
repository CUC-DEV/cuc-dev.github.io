title: 第三次项目例会曾䶮PPT
tags: 
    - presentation
type: presentation
date: 2015-10-23
---
{% raw %}
<section>
    <h1>新媒体项目会议</h1>
    <h3>第三次项目例会</h3>
    <p>
        <small>2015年10月18日</small>
    </p>
</section>
<section>
    <section>
        <h2>上周总结</h2>
    </section>
    <section>
        <ul>
            <li>配置虚拟机</li>
            <li>Daily报告</li>
            <li>JavaScript 单元测试</li>
            <li>Git学习（2）</li>
        </ul>
    </section>
    <section>
        <h2>配置虚拟机</h2>
        <ul>
            <li class="fragment">Linux基本命令</li>
            <li class="fragment">Github SSH配置</li>
            <li class="fragment">Nvm nodejs版本控制</li>
            <li class="fragment">疑问？</li>
        </ul>
    </section>
    <section>
        <h2>Daily报告</h2>
        <small class="fragment">情况非常不错，大家继续保持</small>
        <table>
            <thead>
                <tr>
                    <th>姓名</th>
                    <th>报告数量</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>应泽峰</td>
                    <td>5</td>
                </tr>
                <tr>
                    <td>傅思喆</td>
                    <td>4</td>
                </tr>
                <tr>
                    <td>仇紫荷</td>
                    <td>4</td>
                </tr>
                <tr>
                    <td>曾䶮</td>
                    <td>3</td>
                </tr>
            </tbody>
        </table>
    </section>
    <section>
        <h2>JavaScript单元测试</h2>
        <ul>
            <li class="fragment">Code编辑器：git，task</li>
            <li class="fragment">Mocha</li>
            <li class="fragment">NodeJS Module</li>
            <li class="fragment">疑问？</li>
        </ul>
    </section>
     <section>
        <h2>Git学习(2)</h2>
        <a href="https://github.com/CUC-DEV/training/tree/test-weekly-meeting-2">小测试</a>
        <p>更改<a href="http://www.faceyourmanga.com/editmangatar.php" target="_blank">Avatar</a></p>
    </section>
    <section>
    <h2>作业统计</h2>
    <table>
        <thead>
            <tr>
                <th>作业</th>
                <th>完成比例</th>
                <th>优秀</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>环境配置</td>
                <td>4/4</td>
                <td>曾䶮，仇紫荷，应泽峰，傅思喆</td>
            </tr>
            <tr>
                <td>JS</td>
                <td>4/4</td>
                <td>仇紫荷，应泽峰，傅思喆</td>
            </tr>
            <tr>
                <td>Git</td>
                <td>2/4</td>
                <td>应泽峰，傅思喆</td>
            </tr>
        </tbody>
    </table>
    </section>
</section>
<section data-background-transition="zoom" data-background="#4d7e65" data-transition="slide">
    <h2>运气大比拼<button class="fragment" id="whoIsLucky" style="width:50px;height:30px;color:red">人品</button></h2>
    <h4 id="who">介绍git</h2>
</section>
<section>
    <h2><a href="/2015/10/17/20151017WeeklyPlanning/" target="_blank">下周任务</a>简介</h2>
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
        $("#who").text(who+"介绍Git");
        $("#whoIsLucky").off('click');
        }, 50);
    }
</script>
{% endraw %}
