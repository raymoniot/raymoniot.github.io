---
title: Event Center
description: Summarizes alarming plants and devices and supports creating work orders for events
weight: 1
---

# Function Overview

The Event Center summarizes the plants and devices that have alarmed on the platform: alarms and faults reported by devices generate an event record here. You can search by conditions, and [create a work order]({{< ref "ticket/list" >}} "Work Order List") to follow up on events that need handling.

<img src="../../../../photo/docs/ops/event-enter.webp">

The list shows the plant name, device serial number, event time, event level, event code and event content of each event. The search box at the very top allows quick search by event content or device serial number.

## 1. Advanced Search

<img src="../../../../photo/docs/ops/search.webp">

Supports searching by event level, event time, plant name, device serial number, event code and event content

- **Event level**: 1, 2 and 3 correspond to low, warning and severe respectively, and multiple selections are allowed. Which levels an account can see is determined by the member's "Event Grade Available" (see "Organization Management → Organizational Structure")
- **Event time**: Filter by the interval of the event start time

## 2. Create Work Order

<img src="../../../../photo/docs/ops/ticket.webp">

<img src="../../../../photo/docs/ops/ticket1.webp">

Create a work order for a single event

The work order automatically carries the plant, device, event code and occurrence time of the event. After submission, you can track and handle it in the [Work Order List]({{< ref "ticket/list" >}} "Work Order List").
