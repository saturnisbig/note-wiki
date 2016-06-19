title: 简单的爬虫
slug: parser 
date: 2012-07-22
category: test
tags: python, HTMLParser, urllib2


之前就一直在想怎么把QQ空间的个人日志抓取下来，然后插入到自己写的博客里面。
这样就可以把原来写的东西保留下来，而继续创作新的日志。今天上网搜了一下，
有人写了这样一个程序。urlTo..这个程序抓取的是手机版Qzone上的日志，存取了图
片信息，还对日志的回复做了处理（用json存储？）。

从作者的博客及里面提及的内容看，抓取网页内容主要用这么几个过程。
1.分析要抓取页面的url信息，找出其中一致的地方，用正则表达式表示出这个pattern.
2.调用urllib2模块，抓取url的内容，作处理，保存到本地。

## 用到的Python模块
urllib2
HTMLParser(用于对抓取的页面作处理，可以取得标签内容等)
re
os

## 学到的Python语法
list的extends操作与append的区别: append是添加新的，extends区别扩展list。



参考：

