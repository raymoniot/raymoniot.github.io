---
title: Collector
description: "Collector import and list management, and its details page: alarms, unbinding, changes, upgrade."
weight: 1
---

# Function Overview

The collector is the core device for platform data access: on-site inverters, batteries, meters, optimizers and other **sub-devices** all hang under the collector, and the collector collects and reports their data to the platform in a unified way. So the collector must be imported first and then bound to a plant, and only then can the data of the sub-devices under it be displayed normally.

## 1. Device List

<img src="../../../../photo/docs/device/collector/device-list.png">

The device list can view online, faulty, offline and all device information. The status tabs at the top also show the device count of each status, and clicking a tab shows only the devices in that status:

- **Online**: the device reports data normally
- **Fault**: the device has an unrecovered alarm
- **Offline**: the device has not reported data for a long time

<img src="../../../../photo/docs/device/collector/collector-uninstall.png">

<img src="../../../../photo/docs/device/collector/collector-install.png">

For collector devices, there are two additional statuses

- **Installed**: the collector has been bound to a plant after being imported
- **Not Installed**: the collector has not been bound to a plant after being imported

The list also shows the serial number, firmware version, signal strength, plant, alias, timezone, data update time and so on; click the serial number to enter the collector details page.

Signal strength can be used to judge the network quality on site; refer to the following values:

- Above 80%: good network
- 50%~79%: normal network
- 31%~49%: poor network, barely usable
- 11%~30%: very poor network, optimize it as soon as possible
- Below 10%: disconnected, the network needs to be configured again

## 2. Collector Import

<img src="../../../../photo/docs/device/collector/import-one.png">

The collector import records the collector into the platform, and there are two ways

- Single import: import a single collector, one collector at a time
- Batch import: import multiple collectors at one time by writing the collector SNs into a template file

### 2.1 Single Import

<img src="../../../../photo/docs/device/collector/import-one1.png" width="600" height="450">

Generally, select WI-FI Stick as the collector type.

- **Authorized user**: after filling it in, this user has the view and management permission of the device; if it is left blank, the current logged-in user is used by default
- **Tag**: add remarks to the collector for easy daily classification

### 2.2 Batch Import

<img src="../../../../photo/docs/device/collector/import-more1.png" width="600" height="450">

Download the collector import template

<img src="../../../../photo/docs/device/collector/import-more.png">

You can fill in multiple collector SNs, Owner is the authorized user, Keywords is the tag

<img src="../../../../photo/docs/device/collector/import-more2.png" width="700" height="550">

Select WI-FI Stick as the type, upload and read it for verification, and the addition succeeds; if a wrong SN or an SN that has already been imported is uploaded, the error messages will be listed

## 3. Batch Set Access Authorization

<img src="../../../../photo/docs/device/collector/access.png">

You can check a single device or multiple devices

<img src="../../../../photo/docs/device/collector/access1.png" width="700" height="550">

Enter the email address of the platform account; if it exists, the corresponding platform account will pop up

<img src="../../../../photo/docs/device/collector/access2.png" width="700" height="550">

Select the platform account and click OK to set it successfully

Access authorization grants the view and management permission of the device to other accounts; the authorized accounts can see and manage these devices in their own device lists. The authorized users and management users of a device can perform access authorization, tag and delete on the device in the operation column of the list.

## 4. Batch Set Tags

<img src="../../../../photo/docs/device/collector/tag.png">

<img src="../../../../photo/docs/device/collector/tag2.png">

Tag multiple collectors in a unified way; tags are used to add remarks to devices (for example the installation area and the purpose), which makes daily classification and searching easier.

## 5. Batch Delete

<img src="../../../../photo/docs/device/collector/tag.png">

After checking multiple collectors, you can delete them in batches. **An installed collector (already bound to a plant) cannot be deleted directly**; you need to unbind it on the details page first. After deletion, the device and its data will no longer be displayed, so please operate with caution.

## 6. Single Access Authorization/Set Tag/Delete

<img src="../../../../photo/docs/device/collector/single.png">

The operation column on the right side of the list has three icon buttons, which are "Access Authorization", "Tag" and "Delete" in order; only the authorized users and management users of the device can see and operate them.

## 7. Firmware Version Number Search

<img src="../../../../photo/docs/device/collector/search.png">

Filter devices by firmware version, which makes it easy to confirm which devices need a firmware upgrade.

## 8. Collector Details Page

<img src="../../../../photo/docs/device/collector/detail-enter.png">

You can enter the device details page from the device in the device list

<img src="../../../../photo/docs/device/collector/detail.png">

The collector details page includes the basic information of the collector and its sub-devices; the supported sub-devices include inverters, BMS, optimizers, meters, etc.

The top of the page shows the device name and the time of the latest data update (including the timezone where the device is located); "Alarm" and "Unbind" on the right are the common operations, and the other operations are in the "…" menu. The basic information includes the serial number, alias, status, plant, firmware version, model, communication type, maximum connection quantity, status code, data upload interval and so on.

### 8.1 Alarm

<img src="../../../../photo/docs/device/collector/alert.png">

Alarm opens the device event page of the device, where you can see all the alarms and faults generated by the device, and filter by event grade, event time, event code, event content and other conditions; each event can be viewed in detail, or you can directly create a work order to follow it up.

<img src="../../../../photo/docs/device/collector/alert1.png">

### 8.2 Unbinding

<img src="../../../../photo/docs/device/collector/unbind.png">

Unbinding a collector unbinds the plant bound to the collector; **unbinding a sub-device will delete the sub-device from the collector and clear the data of the sub-device**.

A collector that is not bound to a plant has nothing to unbind, and the unbind button is not clickable.

### 8.3 Other Functions

<img src="../../../../photo/docs/device/collector/other-function.png">

Click "…" in the upper right corner to expand the remaining operations, including changes, create a new work order, alias editing, firmware upgrade, parameter settings and operation log.

### 8.3.1 Changes

<img src="../../../../photo/docs/device/collector/update.png" width="600" height="450">

Change the model and serial number of the collector. If the model or the serial number was filled in incorrectly when importing, you can correct it through changes.

### 8.3.2 Create a New Work Order

<img src="../../../../photo/docs/device/collector/ticket.png" width="600" height="450">

Create a work order for this collector. The work order carries the device information, and the created work order can be viewed and processed in "Operation and Maintenance Center → Work Order System".

### 8.3.3 Alias Editing

<img src="../../../../photo/docs/device/collector/name.png" width="600" height="450">

You can name the collector. The alias is displayed in the device list, the details page and other places; it is recommended to fill in a name that is easy to identify (for example the installation location), and the serial number of the device is not affected.

### 8.3.4 Firmware Upgrade

<img src="../../../../photo/docs/device/collector/ota.png">

Perform an OTA upgrade on the collector: upload the firmware, select the firmware and click Upgrade Now. For the description of the upgrade process and the timeout, refer to the firmware upgrade in "Toolbox → Remote Interaction".

### 8.3.5 Operation Log

<img src="../../../../photo/docs/device/collector/ops.png">

The operation log saves the recent remote interaction records of the device, including OTA, parameter settings and command transmission
