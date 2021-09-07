---
title: "支付系统 - 对账功能设计与实现"
date: 2021-08-31T09:14:00+08:00
lastmod: 2021-08-31T09:14:00+08:00
draft: true
tags: ["Reconciliation","Payment"]
categories : ["Payment"]
author: "Jaswine"

weight:
mathjax: true
autoCollapseToc: true
---

对账功能是每一个支付平台都需要具备的功能。在整个支付系统中，对账功能属于比较简单的功能，并且对数据没有侵入性。

# 1.功能需求

对于支付系统产生的交易记录进行核销，输出对账的记录和平台的对账单。整个对账功能主要分为两个部分:

- 和渠道对账
- 出具对账结果

整个流程如下:


![flow](http://www-jaswine.oss-cn-shanghai.aliyuncs.com/Site/blog/reconciliation/flow.svg)
<div align="center"><span> pic1.流程图 </span> </div>

# 2.设计




