---
title: Switch Perspective
weight: 1
description: Switch between the three user perspectives; each perspective has a different interface and different functions
---

## What is a perspective

The App provides three usage perspectives and the same account can switch between them at any time. The perspective decides **what you see and what you can do**: the landing page, the bottom navigation and the available entries are all different.

<img src="../../../../photo/docs/app/my/switch.png" style="margin-right: 50px" width="300">

| Perspective | Description in the App | Who it is for |
|---|---|---|
| **Professional Consultant** | I am an equipment manufacturer, dealer, installer or professional consultant | People who manage all plants and devices on the platform |
| **Plant User** | Focus on data with the plant as the focus | People who only care about the data of a plant (e.g. plant owners) |
| **Device User** | Focus on data with the device as the focus | People who only care about the data and debugging of a device |

## How to switch

1. Select "Me" in the bottom menu bar of the App
2. Tap "Switch Perspective"
3. Select the perspective you need among the three cards; the active one has a blue border and a check mark in the lower right corner
4. After switching, the App enters the landing page of that perspective (Professional Consultant goes to the plant list, Plant User goes to a plant overview, Device User goes to a device details page)

## Interface and function differences of the three perspectives

| | Professional Consultant | Plant User | Device User |
|---|---|---|---|
| Page you land on | Plant list (all plants) | Overview of one plant | Details of one device |
| Bottom tabs | Plant / Device / Event / Me | Overview / Statistics / Layout / Me | Realtime / Statistics / Me |
| Device list | The "Device" tab shows all devices, filterable by logger and device status, searchable by serial number | Plant page top-right menu → Device List, showing only the devices of that plant | Device details top-right menu → Switch Device |
| Events | Has an "Event" tab to view the events on the platform | No | No |
| Plant operations | Create Plant / Switch Plant / Add Logger / Network Configuration / Device List | Same as the left | No |
| Device details operations | Parameter Settings / Device Alias / Unbind Device | — | Refresh / Switch Device / Add Logger / Network Configuration / Parameter Settings / Device Alias / Unbind Device |

Detailed description of each perspective:

- [Professional Consultant Perspective]({{< ref "manager-view" >}} "Professional Consultant Perspective")
- [Plant User Perspective]({{< ref "plant-view" >}} "Plant User Perspective")
- [Device User Perspective]({{< ref "device-view" >}} "Device User Perspective")

Note that the "Me" page (user information, change password, languages, network configuration, OTA assistant, local debugging, cache cleanup, ORG toolbox, about, etc.) has the same content in all three perspectives; switching the perspective does not change the data permissions of the account itself.
