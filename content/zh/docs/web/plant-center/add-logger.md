---
title: 添加采集器
description: 在电站下绑定采集器：输入序列号添加或通过模板文件批量添加
weight: 13
---

# 功能概述

添加采集器是把采集器绑定到电站。采集器上报的数据会归到这个电站下，电站的实时功率、发电量等指标才有数据。

添加前需要满足两个条件：

- 采集器已经在「设备中心 → 采集器」完成[采集器入库]({{< ref "../device/collector/#2采集器入库" >}} "采集器入库")，未入库的序列号会提示「SN校验失败」
- 序列号没有重复，已经添加过的序列号会提示「序列号已存在」

添加方式有两种：输入单个序列号，或者通过模板文件批量添加。

## 1.添加采集器入口

从电站列表进入电站的[电站详情页]({{< ref "/pvs/#电站详情页" >}} "电站详情页")，右上角添加采集器

![psv-overview](/../../zh/photo/docs/add-logger/add-logger-enter.webp)

## 2.功能概述

- ### 2.1输入采集器序列号添加

  <img src="/../../zh/photo/docs/add-logger/add-one1.webp" width="550" height="400">

  添加序列号，添加前要先对采集器进行[采集器入库]({{< ref "../device/collector/#2采集器入库" >}} "采集器入库")，已入库则忽略

  <img src="/../../zh/photo/docs/add-logger/add-one2.webp" width="550" height="400">

  点击提交按钮完成采集器添加

  <img src="/../../zh/photo/docs/add-logger/add-one3.webp" width="550" height="400">

- ### 2.2通过模板文件添加

  下载模版collector-import-template.xlsx
  
  <img src="/../../zh/photo/docs/add-logger/add-more1.webp" width="550" height="400">
  
  在模版中添加序列号
  
  <img src="/../../zh/photo/docs/add-logger/add-more.webp" width="550" height="400">
  
  通过模版文件添加
  
  <img src="/../../zh/photo/docs/add-logger/add-more2.webp" width="550" height="400">
  
  确认后提交
  
  <img src="/../../zh/photo/docs/add-logger/add-more3.webp" width="550" height="400">

提交成功即完成绑定，采集器上线后电站开始有数据。设备首次上电到数据正常上报之间会有几分钟的延迟，稍等片刻刷新页面即可看到数据。
