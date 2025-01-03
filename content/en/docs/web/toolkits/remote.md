---
title: Remote Interaction
description: Remote interaction with the collector, including command transmission, firmware upgrade (OTA), parameter setting, operation log, etc.
weight: 4
---

# Function Overview

Send downlink commands to the collector, including firmware upgrade, command transmission, parameter setting

<img src="../../../../photo/docs/toolkits/remote-enter.png">

The remote interaction interface displays the current online collector by default, and can also perform advanced search based on serial number, status, power station, tag, and firmware version number

## 1. Firmware Upgrade (OTA)

<img src="../../../../photo/docs/toolkits/remote-ota.png">

Firmware upgrade includes upgrading the collector and upgrading the sub-device. The upgrade process is the same, but the types of the two devices are different and the firmware used is different

<img src="../../../../photo/docs/toolkits/remote-ota1.png" width="700" height="550">

The firmware list shows all the firmware visible under the current account permissions. You can set the upgrade timeout. If the device has no feedback response outside the timeout, it is considered that the OTA upgrade has timed out.

## 2. Command transparent transmission

<img src="../../../../photo/docs/toolkits/remote-send.png">

<img src="../../../../photo/docs/toolkits/remote-send1.png" width="700" height="550">

There are two formats for command transparent transmission, standard Modbus protocol commands and custom commands. After entering the command, click to generate it immediately. The old version is sent for the old version of the firmware, which can be ignored.

## 3. Parameter settings

<img src="../../../../photo/docs/toolkits/remote-set.png">

<img src="../../../../photo/docs/toolkits/remote-set1.png">

You can set and send a single parameter, or click batch setting to set multiple parameters at the same time

## 4. Operation log

<img src="../../../../photo/docs/toolkits/remote-logs.png">

<img src="../../../../photo/docs/toolkits/remote-logs1.png">

The operation log can query all remote interaction records of a device in a time period, and can also search by operation type