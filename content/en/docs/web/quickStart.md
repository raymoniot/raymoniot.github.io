---
title: Quick Start
description: Quickly use Solarhub, from collector network configuration, collector storage, power station creation, collector addition, network configuration, to data viewing
weight: 2
---

## 1. Collector network configuration

Use SolarhubApp to perform collector network configuration operations. When configuring the network, please ensure that the collector and the network configuration mobile phone are under the **same 2.4Ghz** WiFi.

**Note**: During the operation, please allow the application to obtain Bluetooth, positioning, data and other permissions, and turn on Bluetooth, WiFi, and positioning services, otherwise it may cause **devices to be unable to be selected**, or **network configuration fails**.

<img src="../../../photo/docs/quickStart/wifi.png" style="margin-right: 50px" width="300">

<img src="../../../photo/docs/quickStart/wifi1.png" style="margin-right: 50px" width="300">

<img src="../../../photo/docs/quickStart/wifi2.png" style="margin-right: 50px" width="300">

Click Add Device after Network Configuration, and add network configuration devices by scanning the QR code of the collector/manually entering the collector serial number.

<img src="../../../photo/docs/quickStart/wifi3.png" style="margin-right: 50px" width="300">

<img src="../../../photo/docs/quickStart/wifi4.png" style="margin-right: 50px" width="300">

<img src="../../../photo/docs/quickStart/wifi5.png" style="margin-right: 50px" width="300">

Select the device and start configuration. Select the same 2.4Ghz network as the collector, enter the WiFi password, and start network configuration.

<img src="../../../photo/docs/quickStart/wifi6.png" style="margin: 0 auto" width="300">

After the network configuration is successful, the collector will be online on the platform. You can use the platform's [point query]({{< ref "./toolkits/point-query" >}} "point query") to verify whether the device is online. If the point data can be found and the latest data update time is close to the current time, it means that the device is online normally.

## 2. Add the collector to the library

After the network configuration is completed, add the collector to the library and you can view the device in the device list

<img src="../../../photo/docs/quickStart/import.png">

You can use [single import]({{< ref "./device/collector/#21 single import" >}} "import") or [batch import]({{< ref "./device/collector/#22 batch import" >}} "import")

<img src="../../../photo/docs/quickStart/import1.png">

After importing, you can see the imported device. At this time, the device is not installed

## 3. Create a power plant

<img src="../../../photo/docs/quickStart/add-plant.png">

Select the required business type and create the corresponding power plant. For details, please refer to [Create a power plant]({{< ref "./plant-center/create-plant" >}} "Create a power plant")

## 4. Add a logger

For details, refer to [Add a logger]({{< ref "./plant-center/add-logger" >}} "Add a logger")

## 5. View the details of the power plant/device

<img src="../../../photo/docs/quickStart/plant.png">

<img src="../../../photo/docs/quickStart/device.png">

<img src="../../../photo/docs/quickStart/device1.png">