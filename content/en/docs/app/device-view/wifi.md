---
title: Network Configuration
weight: 4
description: Configure the WiFi network for the logger
---

# Function Overview

Tap "Network Configuration" in the menu in the upper right corner of the device details page to configure the WiFi network the logger should connect to. The logger can connect to the server and report data only after the network configuration succeeds.

<img src="../../../../photo/docs/app/device/deviceview-wifi.png" style="margin-right: 50px" width="300">

## How to Use

<img src="../../../../photo/docs/app/my/config1.png" style="margin-right: 20px" width="300">

<img src="../../../../photo/docs/app/my/wifi3.png" style="margin-right: 0px" width="300">

1. On the device details page, tap the menu in the upper right corner and select "Network Configuration" to enter the network configuration interface
2. Tap add device in the upper right corner, and add the logger to be configured by scanning the code or manually entering the serial number
3. The device can be checked only when the logger has entered the network configuration state; after checking it, you enter the Wi-Fi selection interface

<img src="../../../../photo/docs/app/my/wifi4.png" style="margin-right: 20px" width="300">

<img src="../../../../photo/docs/app/my/wifi5.png" style="margin-right: 20px" width="300">

<img src="../../../../photo/docs/app/my/wifi6.png" style="margin-right: 0px" width="300">

4. Select the **2.4GHz** WiFi to connect to and enter the password
5. Tap start network configuration; it usually takes 10s–20s to succeed. After that, the logger goes online on the platform and starts to report data

## Notes

- Before configuring the network, turn on **Bluetooth, WiFi and location** on the phone, and allow the App to access permissions such as Bluetooth and location; otherwise the device may not be found or the network configuration may fail
- The logger only supports **2.4GHz** WiFi; please make sure the phone is connected to the same network
- During network configuration, make sure the logger is powered and in the network configuration state (indicator blinking)
- The flow is exactly the same as "My → Network Configuration", so you can also enter network configuration from "My", see [Network Configuration]({{< ref "../my/config" >}} "Network Configuration")

> Related documents: [Quick Start]({{< ref "../quickStart" >}} "Quick Start") (the complete flow of logger network configuration, import, and binding to a plant)
