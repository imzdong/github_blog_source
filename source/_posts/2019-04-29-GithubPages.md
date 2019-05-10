---
title: 两步完成GitHub搭建个人博客
date: 2019-04-29 16:01:33
categories: 
- 技术
tags:
- GitHubPages
---

两步快速使用github搭建个人博客，借助第三方平台，博客服务器归第三方，自己仅控制博客的控制权（借助GitHub Pages+[Hexo](https://hexo.io/zh-cn/docs/index.html)）
<!-- more -->
### 一、为何要搭建个人博客？
&emsp;&emsp;网上某大神说过“建站三阶段”（针对博客服务器及博客控制权区分）：
> + 1、借助第三方平台，完全把控制权给第三方（比如博客园、CSDN、简书等平台）
> - 2、自己搭建平台，博客服务器及博客控制权都自己来维护（阿里云+网站）
> + 3、借助第三方平台，博客服务器归第三方，自己仅控制博客的控制权（借助GitHub Pages+[Hexo](https://hexo.io/zh-cn/docs/index.html)）

&emsp;&emsp;本人看后，微微一笑，双手赞成。本人已经经历了一二阶段。现在入坑第三阶段。谈谈自己的历程感受吧！**第一阶段：限制太多，不够灵活(最主要广告贼多).第二阶段：太耗时，还耗钱。第三阶段：通过第三方平台，自己自定义网站模板，贼舒服。**这次借助自己建站的机会写下此文。
### 二、GitHub搭建个人博客
&emsp;&emsp;注：在建站之前你要在[GitHub](https://github.com/)有账号。简单提一句：[GitHub](https://github.com/)是通过git进行版本控制的的软件源代码托管服务。可以理解为就是一个云仓库，你可以通过git向仓库提交你想提交的任何文件。
**GitHub搭建的个人博客(本质也就是仓库)**
##### 1、创建仓库
![创建仓库](/images/article/github/1.jpg)
##### 2、仓库命名
![创建仓库](/images/article/github/2.jpg)
###### 2.1、注意空间名称
![创建仓库](/images/article/github/3.jpg)
以上二步操作完，，一个简单的个人博客基本上已经成功了。访问https://xxxx.github.io/
我的https://imzdong.github.io/
![成功](/images/article/github/4.jpg)
> 如果你本人首次操作的时候一定要遵循图片中的提示。老司机随意。最后会讲如果不按照图片提示操作会出现的情况
##### 3、选择简单模板
![简单模板](/images/article/github/5.jpg)
目前两大静态博客主流框架：[Jekyll](http://jekyllcn.com/)和[Hexo](https://hexo.io/zh-cn/)
###### 3.1、github默认主题[Jekyll](http://jekyllcn.com/)
![简单模板](/images/article/github/6.jpg)
###### 3.2、[Jekyll](http://jekyllcn.com/)的几种主题
![简单模板主题](/images/article/github/7.jpg)
###### 3.3、确认主题
简单主题选择完后，再次访问你的网站https://xxxx.github.io/
![简单模板](/images/article/github/8.jpg)
> 注意：**以下是未按照我截图的仓库名称命名出现的问题**

##### 4、注意事项
仓库名称随便起（比如：imzdong） 那需要访问 http://imzdong.github.io/imzdong 才能访问到我的网站
访问 http://imzdong.github.io  是访问不到的
![简单模板](/images/article/github/9.jpg)
![简单模板](/images/article/github/10.jpg)

以上几步就可以简单的实现搭建简易博客了，祝各位好运！欢迎访问[我的博客](https://imzdong.github.io/)
> ##### 参考
[Hexo中文文档](https://hexo.io/zh-cn/docs/index.html)
[Jekyll中文文档](http://jekyllcn.com/)
[我的博客主题文档](https://godbmw.com/passages/2018-11-15-theme-bmw-docs-zh/)