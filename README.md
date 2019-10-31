# git-learning

本仓库主要用于Git学习和常见问题记录，希望大家能在这里学习到更多的Git知识



## 使用帮助文档

```
git help
git help xxx
git xxx --help
git xxx -h
```



## Git创建

创建本地仓库：git init

	$git init
	Initialized empty Git repository in E:/temp/Git/.git/

从远程克隆代码：git clone

	$git clone --recursive https://github.com/chenpeihua/git-learning.git
	Cloning into 'git-learning'...
	remote: Enumerating objects: 3, done.
	remote: Counting objects: 100% (3/3), done.
	remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
	Unpacking objects: 100% (3/3), done.



## Git基本知识

Git工作区参考下图

![](.\image\git-workspace.png)



Git文件状态

![](.\image\git-file-status.png)



## Git 分支

常用命令

* git branch查看本地分支
* git branch -r //查看远程所有分支
* git branch -a //查看本地和远程的所有分支
* git branch <branch-name> //新建分支
* git branch <branch-name> <start-point>//从start-point新建分支
* git branch -d <branch-name> //删除本地分支
* git branch -m <old-branch> <new-branch> //重命名本地分支
* git checkout branch-name //切换分支
* git checkout –b branch-name //创建分支并切换到分支
* git branch -d -r <branch-name> //删除远程分支，删除后还需推送到服务器
* git push origin:<branch-name> //推送至服务器

创建一个Git分支