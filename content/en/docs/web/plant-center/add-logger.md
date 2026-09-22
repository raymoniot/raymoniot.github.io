---
title: Add Collector
description: "Bind a collector to a plant: add by serial number or import in bulk via a template file"
weight: 13
---

# Function Overview

Adding a collector means binding a collector to a plant. The data reported by the collector is attributed to this plant, and only then do indicators such as the plant's Real-time Power and Power Generation have data.

Two conditions must be met before adding:

- The collector has already completed [Collector import]({{< ref "../device/collector/#2-collector-import" >}} "Collector import") in "Device Center → Collector"; a serial number that has not been imported will prompt "SN verification failed"
- The serial number is not duplicated; a serial number that has already been added will prompt "Serial number already exists"

There are two ways to add: enter a single serial number, or add in bulk via a template file.

## 1. Add Collector Entry

From the Plant List, enter the plant's [Plant details page]({{< ref "/pvs/#plant-details-page" >}} "Plant details page"), and add a collector in the upper right corner

![psv-overview](../../../../photo/docs/add-logger/add-logger-enter.webp)

## 2. Function Overview

- ### 2.1 Add by Entering the Collector Serial Number

  <img src="../../../../photo/docs/add-logger/add-one1.webp" width="550" height="400">

  Add the serial number. Before adding, the collector must first undergo [Collector import]({{< ref "../device/collector/#2-collector-import" >}} "Collector import"); ignore this if it has already been imported

  <img src="../../../../photo/docs/add-logger/add-one2.webp" width="550" height="400">

  Click the Submit button to complete adding the collector

  <img src="../../../../photo/docs/add-logger/add-one3.webp" width="550" height="400">

- ### 2.2 Add via Template File

  Download the template collector-import-template.xlsx
  
  <img src="../../../../photo/docs/add-logger/add-more1.webp" width="550" height="400">
  
  Add serial numbers in the template
  
  <img src="../../../../photo/docs/add-logger/add-more.webp" width="550" height="400">
  
  Add via the template file
  
  <img src="../../../../photo/docs/add-logger/add-more2.webp" width="550" height="400">
  
  Submit after confirmation
  
  <img src="../../../../photo/docs/add-logger/add-more3.webp" width="550" height="400">

Once submitted successfully, the binding is complete, and the plant starts to have data after the collector goes online. There will be a delay of a few minutes between the device being powered on for the first time and the data being reported normally; wait a moment and refresh the page to see the data.
