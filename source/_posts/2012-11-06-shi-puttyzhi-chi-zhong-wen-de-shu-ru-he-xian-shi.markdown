---
layout: post
title: "使putty支持中文的输入和显示"
date: 2012-11-06 23:34
comments: true
categories: [putty, tips] 
---
<ol>
<li>启动putty</li>
<li>Category中选择Window - Appearance - Font settings - Font 
中选择Fixedsys字体,
字符集选择CHINESE_GB2312</li>
<li>Category中选择Window - Appearance - Translation - Character set translation中Remote character set设置为UTF-8</li>
<li>在shell中输入export LC_ALL='zh_CN.utf8'</li>
</ol>

