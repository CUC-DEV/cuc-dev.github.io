title: 配置远程Linux服务器SSH密钥认证自动登录
date: 2016-04-25 13:54:16
tags: [ssh,qiuzihe]
---
# 1.在本地机器创建公钥
### $ ssh-keygen -t rsa -C  'your email@domain.com'
-t 指定密钥类型，默认即 rsa ，可以省略
-C 设置注释文字，比如你的邮箱
之前配置过github的ssh,这个文件应该是生成过的，所以可以直接跳过这一步。
 
# 2. 将公钥复制到ssh服务器
### $ ssh-copy-id dev@neomedia.top
![公钥复制到服务器](/img/ssh/1.png)
[ssh-copy-id](http://man.linuxde.net/ssh-copy-id)命令可以把本地主机的公钥复制到远程主机的authorized_keys文件上，ssh-copy-id命令也会给远程主机的用户主目录（home）和~/.ssh, 和~/.ssh/authorized_keys设置合适的权限。
如果成功的话，可以尝试，下面这条命令，不需要输入密码即可链接阿里云服务器
### $ ssh dev@neomedia.top
![链接服务器](/img/ssh/2.png)
# 3. 快捷登录
完成以上步骤后，即可使用以下命令直接登录ssh服务器，再也不用担心你记不住密码了
### $ vim ~/.ssh/config
![打开编辑配置文件](/img/ssh/3.png)
添加下面内容
![为config文件添加内容](/img/ssh/4.png)
# 4.尝试登录
### $ ssh neomedia
![登录成功](/img/ssh/5.png)

# 5.ssh-copy-id使用非默认22端口
连接实验室服务器是使用3333端口,第一步也是将密钥上传到服务器
### $ ssh-copy-id -i ~/.ssh/id_rsa.pub -p 3333  dev@neomedia.top
然后测试一下是不是密钥传输成功
### $ ssh -p 3333 dev@neomedia.top
![登录成功](/img/ssh/6.png)
设置快捷登录，修改config配置文件
### $ vim ~/.ssh/config
![为config文件添加内容](/img/ssh/7.png)
尝试登录
### $ ssh dev
![登录成功](/img/ssh/8.png)

# 6.备注
* 1.每次尝试登录后不要忘记exit退回到当前主机再进行下一步操作。（如果忘记当前终端在哪台服务器上可以利用ifconfig查看一下ip地址）
* 2.config文件内容方便大家复制。
Host neomedia
    HostName neomedia.top
    PreferredAuthentications publickey
    IdentityFile ~/.ssh/id_rsa
    User dev
Host dev
    HostName neomedia.top
    PreferredAuthentications publickey
    IdentityFile ~/.ssh/id_rsa
    Port 3333
    User dev
* 3.帐户名和密码见印象笔记。
