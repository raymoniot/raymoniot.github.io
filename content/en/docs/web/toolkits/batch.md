---
title: Batch Operation
description: "Batch operation: firmware upgrade, parameter settings, command transmission; redo failed devices"
weight: 2
---

# Function Overview

Perform parameter settings, firmware upgrade, command transmission and other operations on devices in batch.

<img src="../../../../photo/docs/toolkits/batch-enter.webp">

A batch operation is organized by "task": first add devices to the task, then select the operation content and submit it. The platform executes device by device and counts the number of successes and failures; failed devices can be redone. Each row in the list displays the task's failed/successful/processing/total counts, operation content, creator and creation time.

## 1. Create Task

<img src="../../../../photo/docs/toolkits/batch-add.webp">

<img src="../../../../photo/docs/toolkits/batch-add1.webp" width="700" height="550">

Devices can be filtered according to the specified device type and plant.

First filter out the target devices by status, device type, program version, serial number and plant name (left column); check them and click "Add" to put them into the right column, which are the devices to be operated in this task.

<img src="../../../../photo/docs/toolkits/batch-add2.webp" width="700" height="550">

Select the device type, select the device in the device list, and add the device.

<img src="../../../../photo/docs/toolkits/batch-add3.webp" width="700" height="550">

Select the type of batch operation required and submit the task.

There are three task types:

- **Firmware Upgrade**: need to select the firmware to upgrade; the firmware is filtered by device type
- **Parameter Settings**: send the selected parameters all at once
- **Command Transmission**: send the same command to the selected devices

After filling in a name for the task and submitting it, the platform executes device by device in a queue. You can refresh the task list to view the progress.

## 2. Redo Failed Devices

<img src="../../../../photo/docs/toolkits/batch-redo.webp">

If device operations fail in a batch operation task, you can use the redo function to redo the failed devices in the batch task.
