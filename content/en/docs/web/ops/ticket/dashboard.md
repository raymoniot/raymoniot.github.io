---
title: Work Order Dashboard
description: "Work Order Dashboard: key counts, today's trend, to-dos and scores"
weight: 2
---

# Function Overview

The Work Order Dashboard is used to quickly understand the overall status of work orders: four key metrics at the top, a work order trend chart in the middle, and to-dos and score statistics below.

<img src="../../../../../photo/docs/ops/ticket/ticket.png">

- **Unresolved**: the number of work orders that are not yet resolved
- **Overdue**: the number of work orders that have passed the first response or close deadline and are still unhandled, which need to be handled first
- **Processing**: the number of work orders being processed
- **Unassigned**: the number of work orders that have not been assigned to a handler

**Today's Trend** compares the change in the number of work orders between yesterday and today. Hover to see the value of a specific period, which helps judge the processing pressure of the day.

**To-do** lists the work orders that need to be handled by the current account; click one to enter that work order directly.

**Score** counts users' evaluations of work order handling results (positive, negative, neutral, unrated), reflecting service quality.

## 1. Recent Activities

<img src="../../../../../photo/docs/ops/ticket/active.png">

<img src="../../../../../photo/docs/ops/ticket/active-expand.png">

Operation records of the work order system

Click "Recent Activities" in the upper right corner to open the drawer, which displays the operation records of work orders in reverse chronological order, including the work order number, operation time, operator and the changed status (such as Open, Pending, Resolved, Closed), making it easy to trace who handled which work order and when.
