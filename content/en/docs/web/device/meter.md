---
title: Smart Meter
description: "Meter list and details page: meter info (voltage, current, power, energy) and micro-inverter data."
weight: 5
---

# Function Overview

The meter is used to measure the energy data of a plant such as the grid connection and the load; it usually hangs under a collector as a sub-device, and the collector collects and reports its data to the platform.

## 1. Device List

<img src="../../../../photo/docs/device/meter/device-list.png">

The device list can view online, faulty, offline and all device information; the status tabs at the top also show the device count of each status, and clicking a tab shows only the devices in that status.

The list shows the serial number, alias, plant, collector, timezone, data update time and so on; click the serial number to enter the meter details page.

## 2. Meter Details Page

<img src="../../../../photo/docs/device/meter/detail-enter.png">

You can enter the device details page from the device in the device list

<img src="../../../../photo/docs/device/meter/detail.png">

The meter details page displays meter information and micro-inverter devices.

The top of the page shows the device name and the time of the latest data update (including the timezone where the device is located); "Alarm" and "Unbind" on the right are the common operations, and the other operations are in the "…" menu. The page content is divided into two parts:

- **Basic information**: smart meter series number, phase A voltage, phase A current, instantaneous total active power, instantaneous total reactive power, grid frequency, forward active total energy, reverse active total energy
- **Micro-inverter devices**: the number of micro-inverter devices under this meter and the serial number of every micro-inverter (SN0, SN1…)

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

### 3.6 Operation Log

Refer to [Operation log for the collector]({{< ref "/collector/#835-operation-log" >}} "Operation Log")
