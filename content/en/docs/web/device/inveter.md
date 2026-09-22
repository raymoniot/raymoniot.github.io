---
title: Inverter
description: "Inverter list and details page: basic info, operation data, faults, parameter settings, charts."
weight: 2
---

# Function Overview

The inverter is the power generation device that converts DC power into AC power; it usually hangs under a collector as a sub-device, and the collector collects and reports its operation data to the platform.

## 1. Device List

<img src="../../../../photo/docs/device/inveter/device-list.png">

The device list can view online, faulty, offline and all device information; the status tabs at the top also show the device count of each status, and clicking a tab shows only the devices in that status.

The list shows the serial number, today's power generation, real-time power, plant, collector, alias, timezone, data update time and so on; click the serial number to enter the inverter details page, and "Plant" and "Collector" can jump to the corresponding pages.

## 2. Advanced Device Search

<img src="../../../../photo/docs/device/inveter/search.png">

The search box supports searching devices by serial number, alias and other keywords; click the search icon to expand the advanced search, where you can query by a combination of multiple device parameters; the specific available query fields are configured by the platform.

## 3. Inverter Details Page

<img src="../../../../photo/docs/device/inveter/detail-enter.png">

You can enter the device details page from the device in the device list

<img src="../../../../photo/docs/device/inveter/detail.png">

The inverter details page displays inverter information and historical data charts.

The top of the page shows the device name and the time of the latest data update (including the timezone where the device is located); "Alarm" and "Unbind" on the right are the common operations, and the other operations are in the "…" menu, including changes, create a new work order, alias editing, firmware upgrade, parameter settings and operation log.

Among the information cards at the top of the page, besides the parameter cards configured by the platform according to the device type, there is also an operation data card (displaying real-time data such as the voltage, current and power of the DC/AC side); the specific content of the parameter cards is configured by the platform and may differ between inverter models, and the parameters an account can see are also limited by the authorized measurement groups (see the description of measurement groups in "Organization Management → Organizational Structure").

### 3.1 Alarm

Refer to [Collector Alarm]({{< ref "/collector/#81-alarm" >}} "Collector Alarm")

### 3.2 Unbinding

Refer to [Collector Unbinding]({{< ref "/collector/#82-unbinding" >}} "Collector Unbinding"), **unbinding a sub-device will delete the sub-device from the collector and clear the data of the sub-device**.

### 3.3 Create a New Work Order

Refer to [Create a new work order for the collector]({{< ref "/collector/#832-create-a-new-work-order" >}} "Create a New Work Order")

### 3.4 Parameter Settings

<img src="../../../../photo/docs/device/inveter/set.png">

Send the measurement point parameter settings through the green button, or click batch settings to send; for details, please refer to the remote interaction link.

Parameter settings are used to deliver writable parameters to the inverter, and the delivery result is recorded in the operation log of the device.

### 3.5 Alias Editing

Refer to [Edit the collector alias]({{< ref "/collector/#833-alias-editing" >}} "Collector Alias Editing")

### 3.6 Firmware Upgrade

Refer to [Firmware upgrade for the collector]({{< ref "/collector/#834-firmware-upgrade" >}} "Firmware Upgrade")

### 3.7 Operation Log

Refer to [Operation log for the collector]({{< ref "/collector/#835-operation-log" >}} "Operation Log")

### 3.8 Historical Data Chart

<img src="../../../../photo/docs/device/inveter/chart.png">

Historical data supports data display and time range selection at the daily, weekly, monthly, yearly and total levels, where different time dimensions display different parameters

- **Daily**: users can customize the parameter display through [Parameter Selection]({{< ref "/inveter/#381-parameter-selection" >}} "Parameter Selection")
- **Weekly**: users can customize the parameter display through [Parameter Selection]({{< ref "/inveter/#381-parameter-selection" >}} "Parameter Selection")
- **Monthly**: display power generation
- **Yearly**: display power generation
- **Total**: display power generation

Above the chart you can select a date or a time range; after switching the dimension, the data is automatically displayed at the corresponding time granularity.

### 3.8.1 Parameter Selection

<img src="../../../../photo/docs/device/inveter/param-select.png">

<img src="../../../../photo/docs/device/inveter/param-select1.png">

Users can select the parameters they want to display and click OK to view them

Parameters are displayed classified by parameter group; check them and click OK to update the chart

<img src="../../../../photo/docs/device/inveter/param-select3.png">

Users can also customize templates, and each template can save its own parameters

A template can save commonly used parameter combinations, so that you can directly select the template next time; a custom template can be renamed by double-clicking its name, and can also be deleted. The range of selectable parameters is likewise limited by the measurement groups authorized to the account.

### 3.8.2 Export Report

<img src="../../../../photo/docs/device/inveter/export.png">

Export the chart data to an Excel table
