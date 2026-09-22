---
title: Remote Interaction
description: "Remote interaction with the collector: command transmission, parameter setting, OTA, operation log"
weight: 4
---

# Function Overview

Send downlink commands to the collector, including firmware upgrade (OTA), command transmission and parameter settings.

<img src="../../../../photo/docs/toolkits/remote-enter.png">

The remote interaction interface displays the currently online collectors by default, and can also perform advanced search by serial number, status, plant, tag and firmware version.

Each row in the list corresponds to a collector, showing status, serial number, brand, model, plant, signal strength, communication type, timezone and data update time. The operation column provides four entries: firmware upgrade, operation log, command transmission and parameter settings.

## 1. Firmware Upgrade (OTA)

<img src="../../../../photo/docs/toolkits/remote-ota.png">

Firmware upgrade includes upgrading the collector and upgrading sub-devices. The upgrade process is the same, but the types of the two devices are different and the firmware used is different.

<img src="../../../../photo/docs/toolkits/remote-ota1.png" width="700" height="550">

The firmware list shows all the firmware visible under the current account permissions. You can set the upgrade timeout; if the device has no feedback response outside the timeout, it is considered that this OTA upgrade has timed out.

The upgrade process and result can be viewed in "Operation Log"; devices that failed or timed out can be upgraded again.

## 2. Command Transmission

<img src="../../../../photo/docs/toolkits/remote-send.png">

<img src="../../../../photo/docs/toolkits/remote-send1.png" width="700" height="550">

There are two formats for the command sent by command transmission: standard Modbus protocol commands and custom commands. After entering the command, click Send Immediately. Old Version Send is used by old firmware and can be ignored.

- **Standard Modbus protocol**: fill in the address, command and data field separately; the tool automatically calculates the CRC16 checksum
- **Custom command**: fill in the complete command directly according to the device protocol

## 3. Parameter Settings

<img src="../../../../photo/docs/toolkits/remote-set.png">

<img src="../../../../photo/docs/toolkits/remote-set1.png">

You can set and send a single parameter, or click Batch Settings to set multiple parameters at the same time.

Each parameter is displayed as a card, containing the point ID, parameter name and input box. After modifying, click the send button on the card to send it separately; when modifying multiple parameters together, click "Batch Settings" at the bottom to send them all at once.

## 4. Operation Log

<img src="../../../../photo/docs/toolkits/remote-logs.png">

<img src="../../../../photo/docs/toolkits/remote-logs1.png">

The operation log can query all the remote interaction records of a device in a time period, and can also search by operation type.

The log records the creation time, processing time, response time, processing result, response code and response result of each interaction, so that you can confirm whether the command was executed successfully.
