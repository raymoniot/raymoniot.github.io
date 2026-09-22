---
title: Production Test
description: "Test devices after production: test standards, test tasks, automatic test report export"
weight: 5
---

# Function Overview

Use production test to test whether a device meets a certain test standard.

Production test is divided into three parts, corresponding to the three tabs on the page:

- **Test Standard**: define "what to measure and what condition counts as passing"
- **Task List**: create test tasks for devices and track their running status
- **Test Record**: the entry for querying historical test tasks and reports

## 1. Create Test Standard

<img src="../../../../photo/docs/toolkits/test.webp">

Select the device type to be tested, select the measurement points, aggregate functions, test conditions and thresholds for testing devices of this type, and save the test standard.

Each measurement point takes one row. You need to select an aggregate function (such as latest value, maximum value) and a test condition (such as =, >, >=), and fill in the threshold; when the task runs, whether the device passes is judged according to these conditions.

<img src="../../../../photo/docs/toolkits/test1.webp">

<img src="../../../../photo/docs/toolkits/test3.webp">

After creation, it can be seen in the list.

<img src="../../../../photo/docs/toolkits/test2.webp">

## 2. Create Test Task

<img src="../../../../photo/docs/toolkits/test4.webp">

Select the created test standard, add device serial numbers (**the device has completed network configuration normally and the device has not been imported**), and support adding multiple devices through a template.

<img src="../../../../photo/docs/toolkits/test5.webp">

Save and add to the task queue.

<img src="../../../../photo/docs/toolkits/test6.webp">

The new task can be seen in the list; at this time the task is in the ready state.

<img src="../../../../photo/docs/toolkits/test7.webp">

Refresh the list with the refresh button and you can see that the task is already in the running state.

<img src="../../../../photo/docs/toolkits/test8.webp">

Move the mouse over the test result to see whether the device is reporting data. A green serial number with an uplink time indicates that the device has reported the latest data; combined with the test standard, decide the test time to judge whether to end the task.

<img src="../../../../photo/docs/toolkits/test9.webp">

Click Running to end the task.

<img src="../../../../photo/docs/toolkits/test10.webp">

After ending, the test report is automatically exported; you need to wait a while.

<img src="../../../../photo/docs/toolkits/test11.webp">

After refreshing the list, you can find that the test report has been exported and is in the Completed state.

<img src="../../../../photo/docs/toolkits/test12.webp">

Click Completed to enter the test report. The test report contains information such as the test results; at this point the test ends.

<img src="../../../../photo/docs/toolkits/test13.webp">

The task list displays the creation time, start/end time, test duration and test result of each task, which is convenient for the production line to keep records by batch.
