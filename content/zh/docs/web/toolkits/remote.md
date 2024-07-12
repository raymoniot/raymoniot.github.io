---
title: 远程交互
description: 对采集器进行远程交互功能，包括指令透传、固件升级（OTA）、参数设置、操作日志等
weight: 4
---

# 功能概述

![unload!](/../../zh/photo/docs/toolkits/remote-enter.png)

远程交互界面默认展示当前在线的采集器，也可以根据序列号、状态、所属电站、标签、固件版本号进行高级搜索

## 1.固件升级（OTA）

![unload!](/../../zh/photo/docs/toolkits/remote-ota.png)

固件升级包括升级采集器和升级子设备，升级过程相同，两者设备的类型不同，使用的固件不同

<img src="/../../zh/photo/docs/toolkits/remote-ota1.png" width="700" height="550">

固件列表中展示当前账号权限下可见的所有固件，可以设置升级超时时间，如果设备在超时时间外无反馈回复，则认为此次OTA升级超时

## 2.指令透传

![unload!](/../../zh/photo/docs/toolkits/remote-send.png)

<img src="/../../zh/photo/docs/toolkits/remote-send1.png" width="700" height="550">

指令透传发送的指令格式有两种，发生标准Modbus协议的指令和自定义指令，输入指令后点击立即发生即可，旧版发送为旧版固件使用，忽略即可

## 3.参数设置

![unload!](/../../zh/photo/docs/toolkits/remote-set.png)

![unload!](/../../zh/photo/docs/toolkits/remote-set1.png)

可以进行单个参数的设置与发送，也可以点击批量设置，同时设置多个参数

## 4.操作日志

![unload!](/../../zh/photo/docs/toolkits/remote-logs.png)

![unload!](/../../zh/photo/docs/toolkits/remote-logs1.png)

操作日志可以查询某个设备在一个时间段所有的远程交互记录，也可以按照操作类型搜索
