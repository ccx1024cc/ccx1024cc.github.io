---
title: Hexo-construct
date: 2019-05-31 15:47:36
tags:
- Hexo
---

### 本地安装Hexo

1.首先安装NPM和git，然后本地安装Hexo：

```
npm install -g hexo

```
2.初始化一个文件夹作为相关文件的目录（网站主目录），然后初始化:

```
hexo init
```
3.可以开始使用Hexo，常用命令包括

```
hexo new filename // 创建一篇文章
hexo g //生成HTML
hexo clean // 清空HTML
hexo s // 开启本地服务器
```

### 和github关联

1.在Github上创建名字为XXX.github.io的项目，XXX为自己的github用户名
2.编辑本地的\_config.yml配置文件：
```
deploy:
  type: git
  repo: git@github.com:ccx1024cc/ccx1024cc.github.io.git
  branch: master
```
3.安装插件：

```
npm install hexo-deployer-git save
```
4.使用命令推送

```
hexo deploy
```
