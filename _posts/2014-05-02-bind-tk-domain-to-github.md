---
author: Yanyd
comments: true
layout: post
date: 2/5/2014 4:28:46 PM 
slug: bind-tk-domain-to-github
title: "绑定TK域名到github pages上"
thread: 3
categories: 
- github

tags:
- DNSPod

---

捣鼓了好久才配置成功，之前直接使用跳转的，但那样设置太弱了，而且后面出现了问题。


### 1、注册TK域名

[地址](http://www.dot.tk)，有时会抽风，注册不了，要耐心一点。

### 2、添加CNAME文件

在仓库根目录下添加一个CNAM文件，没有后缀名，里面内容为你的域名(如:test.tk),
不需要添加http/www等前缀。

`ping username.github.io` 记录下IP地址

### 3、添加DNSPod记录

去[DNSPod](http://www.dnspod.cn)注册个账号，添加域名，设置两个A记录。
分别是`@`和`w w w`，ip地址填上个步骤获取的IP地址。

### 4、设置TK域名的DNS

在Csutom DNS里，设置DNS service,添加两条记录f1g1ns1.dnspod.net和f1g1ns2.dnspod.net

### 5、漫长的等待

要全球解析生效，得等上一会了(72h)。
