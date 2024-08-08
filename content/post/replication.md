---
title: "各中间件数据同步方案"
date: 2022-09-27T14:53:40+08:00
lastmod: 2022-09-27T14:53:40+08:00
draft: false
tags: [""]
categories : ["一致性"]
author: "Jaswine"

weight:
mathjax: true
autoCollapseToc: true
---


|中间件|同步方式|引用|
|:-----|:-----|:-----|
|MySQL|从节点读取binLog|https://dev.mysql.com/doc/refman/8.0/en/replication.html|
|MongoDB|从节点读取oplog|https://www.mongodb.com/docs/manual/replication/|
|Redis|从节点读取binLog|https://redis.io/docs/manual/replication/|
|ElaticSearch|从节点读取binLog|https://www.elastic.co/guide/en/elasticsearch/reference/current/xpack-ccr.html|
|kafka|从节点读取binLog|https://kafka.apache.org/documentation/#replication|
|RocketMQ|从节点读取binLog||