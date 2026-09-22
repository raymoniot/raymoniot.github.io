---
title: 生产测试
description: 生产后对设备进行测试：维护测试标准、创建测试任务、自动导出测试报告
weight: 5
---

# 功能概述

通过生产测试测试设备是否满足某种测试标准

生产测试分为三部分，对应页面上的三个标签页：

- **测试标准**：定义"测什么、达到什么条件算通过"
- **任务列表**：给设备创建测试任务并跟踪运行状态
- **测试记录**：历史测试任务与报告的查询入口

## 1.测试标准创建

<img src="/../../zh/photo/docs/toolkits/test.webp">

选择需要测试的设备类型，选择需要测试该类型设备的测点以及聚合函数，测试条件，阈值，保存测试标准

每个测点一行，需要选择聚合函数（如最新值、最大值）和测试条件（如 =、>、>=），并填写阈值；任务运行时按这些条件判断设备是否通过。

<img src="/../../zh/photo/docs/toolkits/test1.webp">

<img src="/../../zh/photo/docs/toolkits/test3.webp">

创建后在列表中可以看到

<img src="/../../zh/photo/docs/toolkits/test2.webp">

## 2.新建测试任务

<img src="/../../zh/photo/docs/toolkits/test4.webp">

选择创建的测试标准，添加设备序列号(**设备已经正常完成配网并且设备未入库**)，支持通过模版添加多个设备

<img src="/../../zh/photo/docs/toolkits/test5.webp">

保存加入任务队列

<img src="/../../zh/photo/docs/toolkits/test6.webp">

在列表中可以看到新建任务，此时任务处于就绪状态

<img src="/../../zh/photo/docs/toolkits/test7.webp">

通过刷新按钮刷新列表看到任务已经处于运行状态中

<img src="/../../zh/photo/docs/toolkits/test8.webp">

鼠标移动到测试结果上可以看到设备是否上报数据，序列号绿色并且携带上行时间说明设备已经上报最新数据，结合测试标准决定测试时间判断是否结束任务

<img src="/../../zh/photo/docs/toolkits/test9.webp">

点击正在运行后可以进行结束任务

<img src="/../../zh/photo/docs/toolkits/test10.webp">

结束后会自动导出测试报告，需要等待一会

<img src="/../../zh/photo/docs/toolkits/test11.webp">

刷新列表后发现测试报告已导出，处于已完成状态

<img src="/../../zh/photo/docs/toolkits/test12.webp">

点击已完成进入测试报告，测试报告中包含测试结果等信息，此时测试结束

<img src="/../../zh/photo/docs/toolkits/test13.webp">

任务列表中会显示每个任务的创建时间、开始/结束时间、测试时长和测试结果，便于产线按批次留档。
