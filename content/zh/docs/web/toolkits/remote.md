---
title: 远程交互
description: 对采集器进行远程交互：指令透传、参数设置、固件升级（OTA）和操作日志
weight: 4
---

# 功能概述

向采集器发送下行指令，包括固件升级（OTA）、指令透传、参数设置。

<img src="/../../zh/photo/docs/toolkits/remote-enter.png">

远程交互界面默认展示当前在线的采集器，也可以根据序列号、状态、所属电站、标签、固件版本号进行高级搜索

列表中的每一行对应一台采集器，显示状态、序列号、品牌、型号、所属电站、信号强度、通讯类型、时区和数据更新时间；操作列提供四个入口：固件升级、操作日志、指令透传、参数设置。

## 1.固件升级（OTA）

<img src="/../../zh/photo/docs/toolkits/remote-ota.png">

固件升级包括升级采集器和升级子设备，升级过程相同，两者设备的类型不同，使用的固件不同

<img src="/../../zh/photo/docs/toolkits/remote-ota1.png" width="700" height="550">

固件列表中展示当前账号权限下可见的所有固件，可以设置升级超时时间，如果设备在超时时间外无反馈回复，则认为此次OTA升级超时

升级过程与结果可以在「操作日志」中查看；升级失败或超时的设备可以重新发起升级。

## 2.指令透传

<img src="/../../zh/photo/docs/toolkits/remote-send.png">

<img src="/../../zh/photo/docs/toolkits/remote-send1.png" width="700" height="550">

指令透传发送的指令格式有两种，发生标准Modbus协议的指令和自定义指令，输入指令后点击立即发生即可，旧版发送为旧版固件使用，忽略即可

- **标准Modbus协议**：按地址、指令、数据域分别填写，工具会自动计算 CRC16 校验
- **自定义指令**：按设备协议直接填写完整指令

## 3.参数设置

<img src="/../../zh/photo/docs/toolkits/remote-set.png">

<img src="/../../zh/photo/docs/toolkits/remote-set1.png">

可以进行单个参数的设置与发送，也可以点击批量设置，同时设置多个参数

每个参数显示为一张卡片，包含测点编号、参数名称和输入框，修改后点击卡片上的下发按钮单独下发；多个参数一起修改时，点击底部的「批量设置」统一下发。

## 4.操作日志

<img src="/../../zh/photo/docs/toolkits/remote-logs.png">

<img src="/../../zh/photo/docs/toolkits/remote-logs1.png">

操作日志可以查询某个设备在一个时间段所有的远程交互记录，也可以按照操作类型搜索

日志中会记录每次交互的创建时间、处理时间、响应时间、处理结果、响应代码和响应结果，便于确认指令是否执行成功。
