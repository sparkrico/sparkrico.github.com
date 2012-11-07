---
layout: post
title: "Android Manifest uses-sdk"
date: 2012-11-07 21:44
comments: true
categories: [Android, guide]
---

```java syntax
<uses-sdk android:minSdkVersion="integer" 
          android:targetSdkVersion="integer"
          android:maxSdkVersion="integer" />
```
<ol>
<li>如果设定了minSdkVersion，小于minSdkVersion的系统将无法在谷歌市场检索到该应用。如果没有设置，则认为它是1</li>
<li>如果没有设置targetSdkVersion则认为他和minSdkVersion相等。</li>
</ol>
<p>遇到一个问题，使用4.1.2作为targetSdkVersion在我的4.1.2系统上Menu无论如何都出不来（未使用ActionBar），换为2.2后就出来了</p>
