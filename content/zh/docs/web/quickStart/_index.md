---
title: 快速开始
description: 快速使用Solarhub，从采集器配网、采集器入库、创建电站、添加采集器、配网、到查看数据
weight: 2
---



## 1.采集器配网

使用SolarhubApp进行采集器配网操作，配网时请保证采集器和配网手机在**同一个2.4Ghz**的WiFi下。

**注意**：操作过程中请允许应用程序获取蓝牙、定位、数据等权限，并开启蓝牙、WiFi、定位服务，否则可能会导致**设备无法选择**，或者**配网失败**。



<img src="/../../zh/photo/docs/quickStart/wifi.png" style="margin-right: 50px" width="300">

<img src="/../../zh/photo/docs/quickStart/wifi1.png" style="margin-right: 50px" width="300">

<img src="/../../zh/photo/docs/quickStart/wifi2.png" style="margin-right: 50px" width="300">

点击配网后添加设备，通过扫码采集器二维码/手动收入采集器序列号来进行添加配网设备。

<img src="/../../zh/photo/docs/quickStart/wifi3.png" style="margin-right: 50px" width="300">

<img src="/../../zh/photo/docs/quickStart/wifi4.png" style="margin-right: 50px" width="300">

<img src="/../../zh/photo/docs/quickStart/wifi5.png" style="margin-right: 50px" width="300">

勾选设备后开始配置，选择与采集器相同的2.4Ghz网络，输入WiFi密码，开始配网。

<img src="/../../zh/photo/docs/quickStart/wifi6.png" style="margin: 0 auto" width="300">

配网成功后采集器将在平台在线，可以通过平台的[测点查询]({{< ref "../toolkits/point-query" >}} "测点查询")来验证设备是否在线，如果可以查到测点数据并且其中最新数据更新时间与当前时间接近，则说明设备正常在线。

## 2.采集器入库

配网完成后将采集器入库后即可在设备列表中查看该设备

![psv-overview](/../../zh/photo/docs/quickStart/import.png)

可以通过[单个导入]({{< ref "../device/collector/#21单个导入" >}} "导入")或[批量导入]({{< ref "../device/collector/#22批量导入" >}} "导入")两种方式

![psv-overview](/../../zh/photo/docs/quickStart/import1.png)

导入后即可看到导入设备，此时设备是未安装状态

## 3.创建电站

![psv-overview](/../../zh/photo/docs/quickStart/add-plant.png)

选择需要的业务类型，创建对应的电站，详细请参考[创建电站]({{< ref "../plantcenter/createplant" >}} "创建电站")

## 4.添加采集器

详细参考[添加采集器]({{< ref "../plantcenter/addlogger" >}} "添加采集器")

## 5.查看电站/设备详情信息

![psv-overview](/../../zh/photo/docs/quickStart/plant.png)

![psv-overview](/../../zh/photo/docs/quickStart/device.png)

![psv-overview](/../../zh/photo/docs/quickStart/device1.png)

