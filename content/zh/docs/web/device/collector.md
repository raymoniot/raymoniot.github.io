---
title: 采集器
description: 采集器的入库与列表管理（状态筛选、访问授权、标签、删除），以及采集器详情页的报警、解绑、变更、新建工单、别名编辑、固件升级和操作日志
weight: 1
---

# 功能概述

采集器是平台数据接入的核心设备：现场的逆变器、电池、电表、优化器等**子设备**都挂在采集器下，由采集器统一采集并上报数据到平台。所以采集器需要先入库、再绑定到电站，它下面子设备的数据才能正常展示。

## 1.设备列表

<img src="/../../zh/photo/docs/device/collector/device-list.webp">

设备列表可以查看在线、故障、离线和全部的设备信息。上方的状态标签会同时显示各状态的设备数量，点击标签可以只看该状态的设备：

- **在线**：设备正常上报数据
- **故障**：设备存在未恢复的告警
- **离线**：设备长时间没有上报数据

<img src="/../../zh/photo/docs/device/collector/collector-uninstall.webp">

<img src="/../../zh/photo/docs/device/collector/collector-install.webp">

对于采集器设备来说，有两种额外的状态

- **已安装**：采集器入库后进行了绑定电站
- **未安装**：采集器入库后未绑定电站

列表中还会显示序列号、固件版本号、信号强度、所属电站、别名、时区、数据更新时间等，点击序列号可以进入采集器详情页。

信号强度可以用来判断现场的网络质量，参考如下数值：

- 80% 以上：网络良好
- 50%~79%：网络正常
- 31%~49%：网络不佳，勉强使用
- 11%~30%：网络很差，注意优化
- 10% 以下：断网状态，需要重新配网

## 2.采集器入库

<img src="/../../zh/photo/docs/device/collector/import-one.webp">

采集器入库是把采集器录入平台，有两种方式

- 单个导入：单个采集器导入，一次导入一个采集器
- 批量导入：通过将采集器SN写入模版文件，一次性导入多个采集器

### 2.1单个导入

<img src="/../../zh/photo/docs/device/collector/import-one1.webp" width="600" height="450">

一般采集器类型选择WI-FI Stick。

- **授权用户**：填写后该用户拥有设备的查看管理权限；不填写则默认当前登录用户
- **标签**：给采集器添加备注信息，便于日常归类

### 2.2批量导入

<img src="/../../zh/photo/docs/device/collector/import-more1.webp" width="600" height="450">

下载采集器导入模版

<img src="/../../zh/photo/docs/device/collector/import-more.webp">

可以填写多个采集器SN，Owner为授权用户，Keywords为标签

<img src="/../../zh/photo/docs/device/collector/import-more2.webp" width="700" height="550">

类型选择WI-FI Stick，上传并读取校验，即可添加成功，若上传错误的SN或者已入库的SN则会列出报错信息

## 3.批量设置访问授权

<img src="/../../zh/photo/docs/device/collector/access.webp">

可以勾选单个或多个设备

<img src="/../../zh/photo/docs/device/collector/access1.webp" width="700" height="550">

输入平台账号的邮箱，如果存在则会弹出对应的平台账号

<img src="/../../zh/photo/docs/device/collector/access2.webp" width="700" height="550">

选择平台账号，点击确定设置成功

访问授权是把设备的查看管理权限授予其他账号，被授权的账号在自己的设备列表里可以看到并管理这些设备；设备的授权用户和管理用户可以在列表操作列中对设备做访问授权、打标签和删除。

## 4.批量设置标签

<img src="/../../zh/photo/docs/device/collector/tag.webp">

<img src="/../../zh/photo/docs/device/collector/tag2.webp">

给多个采集器统一打标签，标签用于给设备添加备注信息（例如安装区域、用途），便于日常归类和查找。

## 5.批量删除

<img src="/../../zh/photo/docs/device/collector/tag.webp">

勾选多个采集器后可以批量删除。**已安装（已绑定电站）的采集器不能直接删除**，需要先在详情页解绑；删除后设备及其数据将不再展示，请谨慎操作。

## 6.单个访问授权/设置标签/删除

<img src="/../../zh/photo/docs/device/collector/single.webp">

列表右侧操作列有三个图标按钮，依次是「访问授权」「标签」「删除」，只有设备的授权用户和管理用户可以看到并操作。

## 7.固件版本号搜索

<img src="/../../zh/photo/docs/device/collector/search.webp">

按固件版本号筛选设备，便于确认哪些设备需要做固件升级。

## 8.采集器详情页

<img src="/../../zh/photo/docs/device/collector/detail-enter.webp">

从设备列表中的设备可以进入设备详情页

<img src="/../../zh/photo/docs/device/collector/detail.webp">

采集器详情页包括采集器的基本信息和其子设备，支持的子设备有逆变器、BMS、优化器、电表等。

页面顶部显示设备名称和最近一次数据更新时间（含设备所在时区），右侧的「报警」「解绑」是常用操作，其余操作在「…」菜单中。基本信息包括序列号、别名、状态、所属电站、固件版本、型号、通讯类型、最大连接数量、状态码、数据上传间隔等。

### 8.1报警

<img src="/../../zh/photo/docs/device/collector/alert.webp">

报警将打开该设备的设备事件页面，可以看到该设备产生的所有告警和故障，支持按事件级别、事件时间、事件代码、事件内容等条件筛选；每条事件可以查看详情，也可以直接创建工单跟进。

<img src="/../../zh/photo/docs/device/collector/alert1.webp">

### 8.2解绑

<img src="/../../zh/photo/docs/device/collector/unbind.webp">

采集器的解绑将解绑采集器绑定的电站，**子设备的解绑将会从采集器下删除该子设备，清空子设备的数据**。

未绑定电站的采集器没有可解绑的内容，解绑按钮为不可点击状态。

### 8.3其他功能

<img src="/../../zh/photo/docs/device/collector/other-function.webp">

点击右上角的「…」展开其余操作，包括变更、新建工单、别名编辑、固件升级、参数设置、操作日志。

### 8.3.1变更

<img src="/../../zh/photo/docs/device/collector/update.webp" width="600" height="450">

变更采集器的型号和序列号。入库时型号或者序列号填写有误，可以通过变更修正。

### 8.3.2新建工单

<img src="/../../zh/photo/docs/device/collector/ticket.webp" width="600" height="450">

对该采集器创建一个工单。工单会带上设备信息，创建的工单可以在「运维中心 → 工单系统」中查看和处理。

### 8.3.3别名编辑

<img src="/../../zh/photo/docs/device/collector/name.webp" width="600" height="450">

可以对采集器命名。别名会显示在设备列表、详情页等位置，建议填写便于识别的名称（例如安装位置），设备的序列号不受影响。

### 8.3.4固件升级

<img src="/../../zh/photo/docs/device/collector/ota.webp">

对采集器进行OTA升级，上传固件后选择固件，点击立即升级。升级过程与超时时间的说明参考「工具箱 → 远程交互」中的固件升级。

### 8.3.5操作日志

<img src="/../../zh/photo/docs/device/collector/ops.webp">

操作日志保存了最近对该设备的远程交互记录，包括OTA、参数设置、指令透传
