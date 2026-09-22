---
title: Optimizer
description: "Optimizer (controller) list and details page: optimizer count, switch status and real-time power."
weight: 4
---

# Function Overview

The optimizer (MLPE) is used to perform independent maximum power point tracking for every module in a PV string; it usually hangs under a collector as a sub-device, and the collector collects and reports its data to the platform.

## 1. Device List

<img src="../../../../photo/docs/device/optimizer/device-list.webp">

The device list can view online, faulty, offline and all device information; the status tabs at the top also show the device count of each status, and clicking a tab shows only the devices in that status.

The list shows the serial number, alias, plant, collector, timezone, data update time and so on; click the serial number to enter the optimizer controller details page.

## 2. Optimizer Controller Details Page

<img src="../../../../photo/docs/device/optimizer/detail-enter.webp">

You can enter the device details page from the device in the device list

<img src="../../../../photo/docs/device/optimizer/detail.webp">

The optimizer controller details page displays the information of the optimizer controller and the switch status of the optimizers.

The top of the page shows the device name and the time of the latest data update (including the timezone where the device is located); "Alarm" and "Unbind" on the right are the common operations, and the other operations are in the "…" menu. The page content is divided into two parts:

- **Basic information**: controller MAC address, quick switch, optimizer quantity, real-time power, cumulative total energy
- **Optimizer**: one record for every optimizer under the controller, showing the name (alias or serial number) and the real-time power; the color represents the status — green is open, red is closed, gray is offline; the upper right corner of the card is the corresponding color legend, which is used to compare the meaning of the colors and is not an operation button. Clicking an optimizer enters its own details page

### 3.1 Alarm

Refer to [Collector Alarm]({{< ref "/collector/#81-alarm" >}} "Collector Alarm")

### 3.2 Unbinding

Refer to [Collector Unbinding]({{< ref "/collector/#82-unbinding" >}} "Collector Unbinding"), **unbinding a sub-device will delete the sub-device from the collector and clear the data of the sub-device**.

### 3.3 Create a New Work Order

Refer to [Create a new work order for the collector]({{< ref "/collector/#832-create-a-new-work-order" >}} "Create a New Work Order")

### 3.4 Parameter Settings

Refer to [Inverter Parameter Settings]({{< ref "/inveter/#34-parameter-settings" >}} "Inverter Parameter Settings")

### 3.5 Alias Editing

Refer to [Edit the collector alias]({{< ref "/collector/#833-alias-editing" >}} "Collector Alias Editing")

### 3.6 Firmware Upgrade

Refer to [Firmware upgrade for the collector]({{< ref "/collector/#834-firmware-upgrade" >}} "Firmware Upgrade")

### 3.7 Operation Log

Refer to [Operation log for the collector]({{< ref "/collector/#835-operation-log" >}} "Operation Log")
