---
title: Work Order List
description: Overview list of all work orders; change status, modify and score; mine, to-dos and related to me
weight: 3
---

# Function Overview

The Work Order List shows all work orders and is divided into several tabs by the relationship with the current account:

- **Created by me**: work orders created by the current account
- **To-do**: work orders that need to be handled by the current account
- **Related to me**: work orders that the current account has participated in (such as being replied to or copied)
- **All**: all work orders within the data permissions of the current account

<img src="../../../../../photo/docs/ops/ticket/ticket-list.png">

The information in the list includes the work order number, subject, work order type, handler (or creator), first response deadline, close deadline, priority, status and operations. The "Quick Search" at the top allows you to quickly locate a work order by keyword.

## 1. Work Order Status Change

<img src="../../../../../photo/docs/ops/ticket/ticket-status.png">

The status needs to be updated in time during work order handling. The statuses are:

- **Open**: the work order has been created and is waiting to be handled
- **Pending**: waiting for user confirmation or additional information
- **Resolved**: the problem has been handled
- **Closed**: the work order is finished

## 2. Work Order Modification

<img src="../../../../../photo/docs/ops/ticket/ticket-update.png">

<img src="../../../../../photo/docs/ops/ticket/ticket-update1.png">

## 3. To-do

<img src="../../../../../photo/docs/ops/ticket/ticket-undeal.png">

Work orders in To-do show a priority (high, medium, low), so that urgent problems can be handled first by priority.

## 4. Related to Me

<img src="../../../../../photo/docs/ops/ticket/ticket-me.png">

## 5. Work Order Score

After a work order is resolved, you can score the handling result (positive, neutral, negative). The score results are counted in the score section of the [Work Order Dashboard]({{< ref "dashboard" >}} "Work Order Dashboard").
