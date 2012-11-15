---
layout: post
title: "最近做了什么,nginx 403"
date: 2012-11-15 23:27
comments: true
categories: [心情,nginx]
---
最近几天没有写博客,弄了一个国内的服务器,去图书馆借了两本书[版本控制之道-使用Git],还有一本[怪诞行为学],还书的时候发现上次借的书还超期了...,看到几个同事都骑车上班,我就把很久不骑的自行车又翻出来了,骑了两天还可以,没有感觉很累,单程12Km,大概用时45分钟,结果是时间上跟坐车差不了多少.

===================================>

最近developer.android.com 访问奇慢，今天出了4.2，可更新ADT也是奇慢，恰好有个国内的服务器，我就上去试了试在服务器上下载android docs压缩包，结果十分快，大概6M/s，瞬间就下完了，想想本地的速度真是10kb/s就不错了.就想试试把android docs放到了国内服务器上，之前在上面装了一个ROR的应用，配置了nginx（目前还不太熟悉），看看能不能在其基础上实现访问android docs。

通过搜索引擎查找，查阅nginx的文档，有个alias可用于把一个指定目录在现有的应用下呈现。

配好了后浏览,发现会显示403禁止访问,查阅资料,估计是权限问题.修改nginx.conf的user属性后还真成功了,算是对nginx有了一个初步的了解.

change user www-data; to user xxxx;

/etc/nginc/nginx.conf
``` 
#user www-data;
user xxxx;
```

alias:Defines a replacement for the specified location. For example, with the following configuration
```
location /i/ {
    alias /data/w3/images/;
}
```
the request of “/i/top.gif” will be responded with the file /data/w3/images/top.gif.
