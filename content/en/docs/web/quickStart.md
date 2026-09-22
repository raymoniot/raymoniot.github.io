---
title: Quick Start
description: "Quick start with Solarhub: collector network configuration, collector import, create plant, add collector, and view data"
weight: 2
---

# Function Overview

If you are new to the platform, follow the five steps below to connect the on-site devices and see the data:

1. Collector network configuration (use the App to connect the collector to the on-site WiFi)
2. Collector import (add the collector to the platform)
3. Create a plant
4. Add collector (bind the collector to the plant)
5. View plant and device data

## 1. Collector network configuration

Use the Solarhub App to configure the network of the collector. During configuration, make sure the collector and the phone are in the **same 2.4GHz** WiFi.

**Note**: during the operation, please allow the application to get the Bluetooth, location and data permissions, and turn on Bluetooth, WiFi and location services, otherwise the **device may not be selectable** or the **network configuration may fail**.



<img src="../../../photo/docs/quickStart/wifi.webp" style="margin-right: 50px" width="300">

<img src="../../../photo/docs/quickStart/wifi1.webp" style="margin-right: 50px" width="300">

<img src="../../../photo/docs/quickStart/wifi2.webp" style="margin-right: 50px" width="300">

Click network configuration and then add a device: add the device to be configured by scanning the QR code of the collector or by entering the serial number of the collector manually.

<img src="../../../photo/docs/quickStart/wifi3.webp" style="margin-right: 50px" width="300">

<img src="../../../photo/docs/quickStart/wifi4.webp" style="margin-right: 50px" width="300">

<img src="../../../photo/docs/quickStart/wifi5.webp" style="margin-right: 50px" width="300">

After selecting the device, start the configuration: choose the same 2.4GHz network as the collector, enter the WiFi password and start the network configuration.

<img src="../../../photo/docs/quickStart/wifi6.webp" style="margin: 0 auto" width="300">

After the network configuration succeeds, the collector goes online on the platform. You can verify whether the device is online with [Point Query]({{< ref "./toolkits/point-query" >}} "Point Query"): if measurement point data can be queried and the last data update time in it is close to the current time, the device is online normally.

## 2. Collector import

After the network configuration, import the collector so that the device can be seen in the device list

<img src="../../../photo/docs/quickStart/import.webp">

You can use [Single import]({{< ref "./device/collector/#21-single-import" >}} "import") or [Batch import]({{< ref "./device/collector/#22-batch-import" >}} "import")

<img src="../../../photo/docs/quickStart/import1.webp">

After the import the device can be seen, and it is in the not installed state

## 3. Create a plant

<img src="../../../photo/docs/quickStart/add-plant.webp">

Choose the required business type and create the corresponding plant; for details refer to [Create Plant]({{< ref "./plant-center/create-plant" >}} "Create Plant")

## 4. Add collector

For details refer to [Add Collector]({{< ref "./plant-center/add-logger" >}} "Add Collector")

## 5. View plant/device details

<img src="../../../photo/docs/quickStart/plant.webp">

<img src="../../../photo/docs/quickStart/device.webp">

<img src="../../../photo/docs/quickStart/device1.webp">

After the steps above, the plant and device data are updated automatically with the reports of the collector. If you need to assign accounts to colleagues and control which parameters they can see, refer to [Organization management]({{< ref "./organization/tree" >}} "Organizational Structure").
