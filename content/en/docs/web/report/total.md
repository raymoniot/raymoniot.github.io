---
title: Summary Data
description: "Plant and device reports: statistics by day, month, year and total, exportable to Excel"
weight: 1
---

# Function Overview

Summary Data summarizes the day, month, year and total data of all plants and all devices, and you can filter the target data by conditions and then export it as an Excel sheet

<img src="../../../../photo/docs/report/report-enter.webp">

On the left you switch between "Plant report" and "Device report". The filters shared by both pages are:

- **Business Type**: Select the business type to be counted (PV system, battery system, Residential Storage, etc.)
- **Report Type**: Day, month, year, total, which determines the granularity of the statistics and the data displayed
- **Time**: Select the corresponding date or time range according to the report type

## 1. Plant Report

<img src="../../../../photo/docs/report/report-plant.webp">

The plant report counts row by row by plant, including the plant name, plant address, plant owner, contact, and data such as Power Generation and income corresponding to the selected report type; when the report type is "day", "month" or "year", each row is the summary value of one plant within that time range.

The "Plant" filter can specify a single plant; when it is not selected, all plants within the scope are counted.

### 1.1 Export

<img src="../../../../photo/docs/report/export.webp">

Click "Export" in the upper right corner to export the report data under the current filter conditions as an Excel sheet.

## 2. Device Report

<img src="../../../../photo/docs/report/report-device.webp">

The device report counts operating data by device, and you need to select the device type and the **Device Serial Number**. The report content includes device-side parameters such as the Firmware Version, total operating time, power-on time this time, data upload interval, data collection interval, connection count, Signal Strength and heartbeat, which are used to verify the operating status and configuration of the device. The query results can likewise be exported.
