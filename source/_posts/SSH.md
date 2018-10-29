title: '设置Github使用SSH连接 '
author: Angelo Guo
date: 2018-10-29 15:16:52
tags:
---
Using the SSH protocol, you can connect and authenticate to remote servers and services. With SSH keys, you can connect to GitHub Enterprise without supplying your username or password at each visit.
* 使用SSH协议连接Github，你可以<font color=#A52A2A>不用每次都输入用户名密码</font>。


### 步骤

0. 检查是否已经有ssh命令: $ cd ~/.ssh
1. 设置git全局用户名: $ git config --global user.name "你的用户名"
2. 生成ssh key: $ ssh-keygen -t rsa -C "你的邮箱"
3. Copy生产的公钥: $ clip < ~/.ssh/id_rsa.pub
4. 到Github中-->点击自己头像下面的settings-->SSH and GPG Keys-->New SSH Key，然后paste到里面并且保存，点击下面的 Add SSH key就成功了。
5. 执行命令: $ ssh -T git@github.com
