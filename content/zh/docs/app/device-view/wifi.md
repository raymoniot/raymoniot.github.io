---
title: 配网
weight: 4
description: 给采集器配置 WiFi 网络
---

# 功能概述

在设备详情页右上角菜单中点击「配网」，可以给采集器配置要接入的 WiFi 网络。配网成功后采集器才能连上服务器并上报数据。

<img src="/../../zh/photo/docs/app/device/deviceview-wifi.png" style="margin-right: 50px" width="300">

## 使用方法

<img src="/../../zh/photo/docs/app/my/config1.png" style="margin-right: 20px" width="300">

<img src="/../../zh/photo/docs/app/my/wifi3.png" style="margin-right: 0px" width="300">

1. 在设备详情页点击右上角菜单，选择「配网」进入配网界面
2. 点击右上角添加设备，通过扫码或手动输入序列号添加要配网的采集器
3. 采集器已进入配网状态时该设备才会显示为可勾选，勾选后进入 Wi-Fi 选择界面

<img src="/../../zh/photo/docs/app/my/wifi4.png" style="margin-right: 20px" width="300">

<img src="/../../zh/photo/docs/app/my/wifi5.png" style="margin-right: 20px" width="300">

<img src="/../../zh/photo/docs/app/my/wifi6.png" style="margin-right: 0px" width="300">

4. 选择要接入的 **2.4GHz** WiFi 并输入密码
5. 点击开始配网，一般等待 10s–20s 即可配网成功；成功后采集器会在平台上在线并开始上报数据

## 注意事项

- 配网前请打开手机的**蓝牙、WiFi、定位**，并允许 App 获取蓝牙、定位等权限，否则可能搜索不到设备或配网失败
- 采集器只支持 **2.4GHz** WiFi，请确认手机连接的也是同一网络
- 配网时请保证采集器已有供电并处于配网状态（指示灯闪烁）
- 配网流程与「我的 → 配网」完全一致，也可以从「我的」进入配网，见[配网]({{< ref "../my/config" >}} "配网")

> 相关文档：[快速开始]({{< ref "../quickStart" >}} "快速开始")（采集器配网、入库、绑定电站的完整流程）
