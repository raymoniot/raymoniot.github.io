---
title: 批量操作
description: 批量对多个设备进行固件升级、参数设置、指令透传：创建任务、查看任务进度、重做失败设备
weight: 2
---

# 功能概述

批量对设备进行参数设置，固件升级，指令透传等操作

<img src="/../../zh/photo/docs/toolkits/batch-enter.png">

批量操作以「任务」为单位：先把设备加到任务里，再选择操作内容提交，平台按台执行并统计成功、失败数量，失败的设备可以重做。列表中的每行显示任务的失败/成功/处理中/全部数量、操作内容、创建者和创建时间。

## 1.创建任务

<img src="/../../zh/photo/docs/toolkits/batch-add.png">

<img src="/../../zh/photo/docs/toolkits/batch-add1.png" width="700" height="550">

可以按照指定设备类型和电站进行设备的筛选

先按状态、设备类型、程序版本、序列号、电站名称筛选出目标设备（左栏），勾选后点击「添加」放入右栏，即为本次任务要操作的设备。

<img src="/../../zh/photo/docs/toolkits/batch-add2.png" width="700" height="550">

选择设备类型，选择设备列表中的设备，添加设备

<img src="/../../zh/photo/docs/toolkits/batch-add3.png" width="700" height="550">

选择需要批量操作的类型，提交任务

任务类型有三种：

- **固件升级**：需要选择要升级的固件，固件按设备类型过滤
- **参数设置**：对选中的参数统一下发
- **指令透传**：对选中的设备发送同一条指令

给任务填写名称并提交后，平台会按队列逐台执行，可以在任务列表中刷新查看进度。

## 2.重做失败设备

<img src="/../../zh/photo/docs/toolkits/batch-redo.png">

如果批量操作任务重出现设备操作失败，可以使用重做功能，对批量任务中失败的设备进行重做
