---
title: Battery System
description: "Battery System list and details page: BMS and battery info, charge/discharge, voltage, temperature."
weight: 3
---

# Function Overview

The Battery System (BMS) is the core device of an energy storage system; it usually hangs under a collector as a sub-device, and the collector collects and reports the operation data of the battery clusters and battery packs to the platform.

## 1. Device List

<img src="../../../../photo/docs/device/battery/device-list.webp">

The device list can view online, faulty, offline and all device information; the status tabs at the top also show the device count of each status, and clicking a tab shows only the devices in that status.

The list shows the serial number, alias, average SOC, plant, collector, timezone, data update time and so on; click the serial number to enter the battery details page.

## 2. Battery Details Page

<img src="../../../../photo/docs/device/battery/detail-enter.webp">

You can enter the device details page from the device in the device list

<img src="../../../../photo/docs/device/battery/detail.webp">

The battery details page displays the BMS information, the battery information under its BMS, and historical data charts.

The top of the page shows the device name and the time of the latest data update (including the timezone where the device is located); "Alarm" and "Unbind" on the right are the common operations, and the other operations are in the "…" menu. The page content is grouped by cards:

- **Basic information**: serial number, host device name, host manufacturer name, host software version, total quantity of batteries
- **Charge/Discharge**: average SOC, minimum SOH, charge/discharge status
- **Voltage & Current**: average voltage, total current, maximum cell voltage, minimum cell voltage, maximum charge current, maximum discharge current
- **Temperature**: BMS maximum temperature, BMS minimum temperature, maximum cell temperature, minimum cell temperature
- **Battery**: each battery (battery pack) has its own card, showing information such as the software version and the voltage details of every cell, and the card can be collapsed; the upper right corner allows unbinding this battery separately

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

### 3.8 Historical Data Chart

<img src="../../../../photo/docs/device/battery/chart.webp">

Battery historical data supports data display and time range selection at the daily and weekly levels

- **Daily**: users can customize the parameter display through [Parameter Selection]({{< ref "/battery/#381-parameter-selection" >}} "Parameter Selection")
- **Weekly**: users can customize the parameter display through [Parameter Selection]({{< ref "/battery/#381-parameter-selection" >}} "Parameter Selection")

### 3.8.1 Parameter Selection

Parameter selection is the same as for the inverter; refer to [Inverter Parameter Selection]({{< ref "/inveter/#381-parameter-selection" >}} "Parameter Selection")

### 3.8.2 Export Report

The export method is the same as for the inverter; refer to [Inverter Export Report]({{< ref "/inveter/#382-export-report" >}} "Export Report")
