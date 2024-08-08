---
title: "Redis持久化的原理及其实现"
date: 2021-08-31T21:46:50+08:00
lastmod: 2021-08-31T21:46:50+08:00
draft: false
tags: ["Redis"]
categories : ["Redis"]
author: "Jaswine"

weight:
mathjax: true
autoCollapseToc: true
---

`Redis`是一个基于内存的K-V数据库，当发生宕机的情况下，存储在`Redis`中的数据也会丢失。`Redis`提供了两种方式来实现数据持久化:

- RDB(Redis Database)
- AOF(Append Only File)

# RDB

RDB实现原理本质上是当执行`SAVE`或者`BGSAVE`命令的时候，立马生成当前数据库的快照文件并保存到磁盘中。RDB有以下的特点:

- 当前Redis数据库数据的全量快照
- 生成的文件是一个二进制的dump文件

## RDB原理

## RDB的dump文件组成及其解析

dump文件是二进制的，不利于查看，可以使用工具`redis-rdb-tools`来查看其中的文件。

```shell
rdb --command json ./Downloads/dump.rdb
```

![](http://www-jaswine.oss-cn-shanghai.aliyuncs.com/Site/blog/redis/dump.png)


- 解析Redis dump文件工具下载:[🔗 redis-rdb-tools](https://github.com/sripathikrishnan/redis-rdb-tools)


-----

# AOF

## AOF原理


# 参考

- [Redis Persistence - Official Document](https://redis.io/topics/persistence)


