---
title: Plant Center
description: "Manage plants: query, add, view, follow, edit, delete and export/refresh plant data"
weight: 6
---

# Function Overview

The Plant Center is divided by business type into pages such as PVS, Battery System, Residential Storage and Commercial Plant. Each page has the same structure:

- **Plant Overview**: summarizes the plant data of this business type under the current account's data permissions into several metrics (real-time power, energy, social benefits, online plants, etc.). Click "System large screen" in the upper right corner to display it in full screen
- **Plant List / Plant Map**: the list lets you view plants by status (online, fault, offline) and supports keyword search by plant name, address, plant owner, etc.; the map displays the online status and distribution of plants by geographic location
- **Add Plant**: create a new plant, for details see [Create Plant]({{< ref "/create-plant" >}} "Create Plant")
- **Plant details page**: click a plant to enter it, view the charts, devices, alarms, layout and info of that plant, and add collectors, create work orders, repair power generation, etc.

Plant data comes from the collectors bound to the plant and their sub-devices, so after creating a new plant you also need to [Add Collector]({{< ref "/add-logger" >}} "Add Collector") before the plant starts to have data.

Which plants you can see in the list and on the details page depends on the account's data permissions (see "Organization Management → Organizational Structure") and whether you are authorized as a visitor (see [Visitor Authorization]({{< ref "/guest-access" >}} "Visitor Authorization")).
