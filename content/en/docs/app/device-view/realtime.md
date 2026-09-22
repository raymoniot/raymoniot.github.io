---
title: Real-time Data
weight: 1
description: Default page after entering the Device User Perspective
---

# Function Overview

After entering the Device User Perspective, the **device details** real-time data page opens by default, showing the current working status and parameters of this device.

<img src="../../../../photo/docs/app/view/device-root.png" style="margin-right: 50px" width="300">

## Page Content

The parameters shown differ by device type; take a Battery System as an example:

- **SN**: the device serial number
- **SOC Status**: remaining capacity, total voltage, etc.
- **State of Health (SOH)**: battery health, cycle count
- **System Power**: current power and charge/discharge status (Charging/Discharging)
- **Total Voltage, Battery Current** and other real-time parameters

## Common Operations

- Upper right menu: Refresh, Switch Device, Add Logger, Network Configuration, Parameter Settings, Device Alias, Unbind Device
- The bottom tabs switch among Real-time, Statistics, and My
- Pull down the page to refresh the data

> Note: the parameters an account can see are limited by the **Measurement Group**. If no parameter or an incomplete set of parameters is shown here, check the measurement group authorization in "Organization management → Organizational Structure" on the Web platform (see [Organizational Structure](../../web/organization/tree/) in the Web documents).
