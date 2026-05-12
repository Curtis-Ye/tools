# 如何设置github SSH
## 第一步：安装ssh
使用命令：*$ sudo apt-get install openssh-server*
## 第二步：生成秘钥
使用命令：*$ ssh-keygen -t rsa -C "your email"* **your email指的是你的邮箱**
**若不需要密码，连续三次回车，在~/.ssh/目录下得到两个文件：id_rsa和id_rsa.pub。**
## 第三步：把id_rsa.pub中的内容复制到github个人主页setting里的SSH里
## 第四步：测试
使用命令：*$ ssh -T git@github.com* **在弹出的信息中选择yes即可**
以上便设置成功