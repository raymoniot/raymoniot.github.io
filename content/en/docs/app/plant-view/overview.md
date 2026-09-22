---
title: Plant Overview
weight: 1
description: Default page after entering the Plant User Perspective
---

# Function Overview

After entering the Plant User Perspective, the **Plant Overview** opens by default, showing the real-time power, generation, and estimated revenue of this plant.

<img src="../../../../photo/docs/app/view/plant-root.png" style="margin-right: 50px" width="300">

## Page Content

- **Top**: plant name, time of the latest data update (with time zone)
- **Plant diagram**: shows the current real-time power and the operating status of components such as PV and grid
- **Generation**: generation (kWh) for the four dimensions of today, this month, this year, and all
- **Estimated Revenue**: estimated revenue for today, this month, this year, and all (displayed in the currency unit configured on the platform)

## Common Operations

- Upper right menu: Create Plant, Switch Plant, Add Logger, Network Configuration, Device List
- The bottom tabs switch among Overview, Statistics, Layout, and My
- Pull down the page to refresh the data

> Note: the overview data comes from the logger bound to this plant and its sub-devices. If no logger is bound to the plant yet, generation and revenue will be shown as `--`. To add a logger, see [Add Logger]({{< ref "logger" >}} "Add Logger").
