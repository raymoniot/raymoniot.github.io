---
title: Point Query
description: "Point Query: query the latest reported data of a device by serial number, and export a day's data"
weight: 1
---

# Function Overview

Query how a device reports measurement point data; the latest data reporting is displayed.

<img src="../../../../photo/docs/toolkits/point-query.webp">

It is used to troubleshoot device-side problems: for example, confirm whether the device is reporting, and whether the reported firmware version, server address, signal strength and other parameters meet expectations. The query result only reflects the **latest data of the current day**.

The query result is displayed one by one by measurement point:

- **Point ID**: the number of the measurement point in the device type
- **Measurement point name**: the name of the measurement point (such as data update time, firmware version, Server Url, upload signal strength, etc.)
- **Measurement point value**: the value or text most recently reported by the device

## 1. Point Query Export

<img src="../../../../photo/docs/toolkits/point-query1.webp">

Enter the device serial number to query the device data.

<img src="../../../../photo/docs/toolkits/point-export.webp">

Select the export time to export the data of a certain day.

The exported data is exported as a spreadsheet file by the selected date, which is convenient for further analysis or handing over to R&D to locate problems.
