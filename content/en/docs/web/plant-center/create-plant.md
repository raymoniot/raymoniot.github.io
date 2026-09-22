---
title: Create Plant
description: "Create a Plant: basic information, geographic location, stakeholders (visitors) and photos"
weight: 10
---

# Function Overview

Creating a plant means entering a plant into the platform and filling in its Installed Capacity, address coordinates, owner, visitors, and other information. After creation, the plant appears in the Plant List, and once a collector is bound, the Power Generation data becomes available.

## 1. Create Entry

<img src="../../../../photo/docs/add-plant/add-plant.webp">

Click "Add Plant" in the upper right corner of the page for the corresponding business type in the Plant Center, and complete the wizard in four steps: Basic Information → Geographic Location → Stakeholders → Photos.

## 2. Complete the Plant Information

### 2.1 Fill in Basic Information

<img src="../../../../photo/docs/add-plant/add-plant1.webp">

- **Business Type**: Determines whether the plant belongs to a PV system, a battery system, Residential Storage or a Commercial Plant. After creation the plant appears on the corresponding page and cannot be modified
- **Plant Type**: Such as household residential, used to further distinguish scenarios
- **Plant Name**: Required; a name that is easy to identify and search is recommended
- **Grid Connect Type**: Such as full grid feed-in, self-consumption, etc.
- **Build Date**: The commissioning date of the plant; you can create the plant without filling it in
- **Unit Income, Total Cost, Currency**: Used to calculate and display plant income; if not filled in, income-related indicators are calculated as 0
- **PV Capacity (kWp) / Battery Storage Capacity (kWh)**: Displayed according to the selected business type. PV plants fill in the PV Capacity; battery system and storage plants also fill in the Battery Storage Capacity. These two items are required for the corresponding business type and are used to calculate indicators such as full-load hours, so please fill them in according to the actual situation

### 2.2 Select the Geographic Location

<img src="../../../../photo/docs/add-plant/location.webp" width="30%">

Allowing the website to locate quickly obtains the current location

<img src="../../../../photo/docs/add-plant/add-plant2.webp">

Select a location on the map to obtain the coordinate information as the plant location

The plant coordinates are used for the display on the Plant Map; it is recommended to fill them in accurately.

### 2.3 Add Stakeholders (Visitors)

<img src="../../../../photo/docs/add-plant/add-plant3.webp">

Entering the visitor's email address authorizes the plant to other accounts on the platform, so that they have access to the plant

- **Plant Owner**: Defaults to the currently logged-in account; the owner can modify and delete this plant
- **Plant Visitor**: The authorized account can see this plant in its own Plant List and view the data, but cannot modify or delete the plant. For the scope of permissions, see [Visitor Authorization]({{< ref "/guest-access" >}} "Visitor Authorization")
- **Contact, Contact Phone**: Record the on-site contact information of the plant

### 2.4 Upload Plant Photos

<img src="../../../../photo/docs/add-plant/add-plant4.webp">

### 2.5 Submit

<img src="../../../../photo/docs/add-plant/add-plant5.webp">

After successful creation, you can see the plant in the Plant List, and you can also [modify]({{< ref "/edit-plant" >}} "Modify Plant") and delete the plant in the operation column of the list

After the plant is created, the next step is to [add a collector]({{< ref "/add-logger" >}} "Add Collector"). Only after the collector reports data will the plant have data such as Real-time Power and Power Generation.
