---
title: 采集器
description: 采集器
weight: 1
---

# 功能概述

## 1.设备列表

![unload!](/../../zh/photo/docs/device/collector/device-list.png)

设备列表可以查看在线、故障、离线和全部的设备信息。

![unload!](/../../zh/photo/docs/device/collector/collector-uninstall.png)

![unload!](/../../zh/photo/docs/device/collector/collector-install.png)

对于采集器设备来说，有两种额外的状态

- **已安装**：采集器入库后进行了绑定电站
- **未安装**：采集器入库后未绑定电站



## 2.采集器入库

![unload!](/../../zh/photo/docs/device/collector/import-one.png)

采集器入库有两种方式

- 单个导入：单个采集器导入，一次导入一个采集器
- 批量导入：通过将采集器SN写入模版文件，一次性导入多个采集器

### 2.1单个导入

<img src="/../../zh/photo/docs/device/collector/import-one1.png" width="600" height="450">

一般采集器类型选择WI-FI Stick，填写授权用户可以将该设备授权给其他用户，该用户拥有设备的查看管理权限，不填写则默认当前登录用户，填写标签会对采集器添加备注信息。

### 2.2批量导入

<img src="/../../zh/photo/docs/device/collector/import-more1.png" width="600" height="450">

下载采集器导入模版

![unload!](/../../zh/photo/docs/device/collector/import-more.png)

可以填写多个采集器SN，Owner为授权用户，Keywords为标签

<img src="/../../zh/photo/docs/device/collector/import-more2.png" width="700" height="550">

类型选择WI-FI Stick，上传并读取校验，即可添加成功，若上传错误的SN或者已入库的SN则会列出报错信息

## 3.批量设置访问授权

![unload!](/../../zh/photo/docs/device/collector/access.png)

可以勾选单个或多个设备

<img src="/../../zh/photo/docs/device/collector/access1.png" width="700" height="550">

输入平台账号的邮箱，如果存在则会弹出对应的平台账号

<img src="/../../zh/photo/docs/device/collector/access2.png" width="700" height="550">

选择平台账号，点击确定设置成功

## 4.批量设置标签

![unload!](/../../zh/photo/docs/device/collector/tag.png)

![unload!](/../../zh/photo/docs/device/collector/tag2.png)

## 5.批量删除

![unload!](/../../zh/photo/docs/device/collector/tag.png)

## 6.单个访问授权/设置标签/删除

![unload!](/../../zh/photo/docs/device/collector/single.png)

## 7.固件版本号搜索

![unload!](/../../zh/photo/docs/device/collector/search.png)

## 8.采集器详情页

![unload!](/../../zh/photo/docs/device/collector/detail-enter.png)

从设备列表中的设备可以进入设备详情页

![unload!](/../../zh/photo/docs/device/collector/detail.png)

采集器详情页包括采集器的基本信息和其子设备，支持的子设备有逆变器、BMS、优化器、电表等。

### 8.1报警

![unload!](/../../zh/photo/docs/device/collector/alert.png) 

报警将打开该设备的设备事件页面，可以看到该设备产生的所有告警

![unload!](/../../zh/photo/docs/device/collector/alert1.png) 

### 8.2解绑

![unload!](/../../zh/photo/docs/device/collector/unbind.png)

采集器的解绑将解绑采集器绑定的电站，**子设备的解绑将会从采集器下删除该子设备，清空子设备的数据**。

### 8.3其他功能

![unload!](/../../zh/photo/docs/device/collector/other-function.png)

### 8.3.1变更

<img src="/../../zh/photo/docs/device/collector/update.png" width="600" height="450">

变更采集器的型号和序列号

### 8.3.2新建工单

<img src="/../../zh/photo/docs/device/collector/ticket.png" width="600" height="450">

对该采集器创建一个工单

### 8.3.3别名编辑

<img src="/../../zh/photo/docs/device/collector/name.png" width="600" height="450">

可以对采集器命名

### 8.3.4固件升级

![unload!](/../../zh/photo/docs/device/collector/ota.png)

对采集器进行OTA升级，上传固件后选择固件，点击立即升级

### 8.3.5操作日志

![unload!](/../../zh/photo/docs/device/collector/ops.png)

操作日志保存了最近对该设备的远程交互记录，包括OTA、参数设置、指令透传

