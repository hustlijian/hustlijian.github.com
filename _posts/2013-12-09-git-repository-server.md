---
layout: post
title: "搭建Git服务器仓库"
categories: git
summary: 使用git可以简单的搭建Git服务器仓库，原理是使用ssh登录，这个方法的优点就是简单。
---

使用git可以简单的搭建Git服务器仓库，原理是使用ssh登录，这个方法的优点就是简单。

参考：[Git教程](http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000) 中git服务器搭建

使用步骤：
----------
##1.安装git：

    sudo apt-get install git

##2.创建一个git用户，用来运行git服务：

    sudo adduser git

##3.创建证书登录：  

收集所有需要登录的用户的公钥，就是他们自己的id_rsa.pub文件，把所有公钥导入到`/home/git/.ssh/authorized_keys`文件里，一行一个。

##4.初始化Git仓库:  

先选定一个目录作为Git仓库，假定是`/home/my_name/repositorys/git-template.git`，在`/home/my_name/repositorys`目录下输入命令：

    sudo git init --bare git-template.git

Git就会创建一个裸仓库，裸仓库没有工作区，因为服务器上的Git仓库纯粹是为了共享，所以不让用户直接登录到服务器上去改工作区，并且服务器上的Git仓库通常都以.git结尾。然后，把owner改为git：  

    sudo chown -R git:git git-template.git

##5.禁用shell登录：

出于安全考虑，第二步创建的git用户不允许登录shell，这可以通过编辑/etc/passwd文件完成。找到类似下面的一行：   

    git:x:1001:1001:,,,:/home/git:/bin/bash

改为：   

    git:x:1001:1001:,,,:/home/git:/usr/bin/git-shell

这样，git用户可以正常通过ssh使用git，但无法登录shell，因为我们为git用户指定的git-shell每次一登录就自动退出。

##6.克隆远程仓库：

现在，可以通过git clone命令克隆远程仓库了，在各自的电脑上运行：  

    git clone git@XXX.XXX.XXX.XXX:/home/my_name/repositorys/git-template.git
	(XXX.XXX.XXX.XXX是服务器的IP)

##7.公钥管理

如果团队很小，把每个人的公钥收集起来放到服务器的/home/git/.ssh/authorized_keys文件里就是可行的。如果团队有几百号人，就没法这么玩了，这时，可以用Gitosis来管理公钥。

##8.使用实例：

- clone工程：`git clone git@192.168.6.80:/home/my_name/repositorys/git-template.git`
- 提交修改：`git push` ，或指定branchs:`git push origin master`
- 更新数据：`git pull`

注：
-------
 1.使用”git init –bare”方法创建一个所谓的裸仓库，之所以叫裸仓库是因为这个仓库只保存git历史提交的版本信息，而不允许用户在上面进行各种git操作，如果你硬要操作的话，只会得到下面的错误（”This operation must be run in a work tree”）
这个就是最好把远端仓库初始化成bare仓库的原因。

