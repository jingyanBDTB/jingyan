---
title: Hexo换电脑后如何继续维护博客
date: 2018-02-05 12:21:29
description: Hexo换电脑后如何继续维护博客
categories: nodejs
tags: Hexo
toc: true
author: Yan
comments: 
original: 
permalink: 
---

## 更换PC后如何继续维护GitHub的博客

直入主题，好多人都在github搭建了自己的静态博客，那么有个问题，再我们更换PC后，如何继续维护博客呢？下面就是一些建议。

个人博客也算是一个项目，作为一个程序员应该明白，一个能运行的项目，从大的方面理论上就分两部分：源码、编译生成的可运行文件。通常我们需要维护的就是源码，上线的是编译好的文件，博客的维护是一个道理。

在搭建完博客，安装完主题后，第一件事就是把这套源码维护起来，当然最方便的就是github了。记得在github创建一个和你用户名一样的仓库，把代码同步上去，这就为完成了第一步。第二步，编译部署。这个大家很熟悉，没什么说的，按照标准的hexo命令来就行。那么当你换了电脑，怎么处理呢，有人会疑问，我重新安装hexo，那我之前的基于主题的配置被覆盖了怎么办？其实没那么麻烦，下面就是更换PC后的操作：

	0： 克隆源码、安装nodejs(准备环境)
	1： npm install -g hexo-cli (安装hexo,切记只需安装，不需要初始化init)
	2： npm install hexo-server --save （安装本地测试的server,新版需要单独安装）
	3： hexo clean （编译两部曲）
	4： hexo generate
	5:  hexo server （本地测试）
	6:  hexo deploy （部署）

是不是发现没你想象那么麻烦，觉得实用就转发吧...

