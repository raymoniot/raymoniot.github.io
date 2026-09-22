---
title: Firmware Management
description: "Device OTA firmware management: search, add, modify, download, access authorization, redemption code"
weight: 1
---

# Function Overview

Platform device firmware management, including firmware search, adding firmware, modifying firmware, downloading firmware, access authorization, generating redemption codes, etc.

<img src="../../../../photo/docs/toolkits/firmware-enter.png">

Firmware is maintained separately by device type (collector, inverter, battery system, battery PACK, micro inverter, etc.). The list displays firmware name, firmware version, extended info, remark, file size and update time. When performing firmware upgrade in remote interaction and on the device details page, only the firmware that the current account has permission for and that matches the target device type will be seen.

## 1. Firmware Search

<img src="../../../../photo/docs/toolkits/firmware-search1.png">

<img src="../../../../photo/docs/toolkits/firmware-search.png" width="700" height="550">

Advanced search can be performed based on device type or firmware name.

## 2. Add Firmware

<img src="../../../../photo/docs/toolkits/firmware-add.png">

<img src="../../../../photo/docs/toolkits/firmware-add1.png" width="600" height="450">

- **Device type**: required, selected in three levels by device type/brand/model; the firmware can only be used for the selected model
- **Firmware name, Firmware version**: required, **firmware version** should not be too long
- **Extended info**: used to distinguish firmware differences under the same model (for example, whether the serial chip is distinguished)
- **Firmware file**: required, the file size cannot exceed 2MB; please make sure the **firmware file is legal**, otherwise it cannot be added
- **Authorize to members of the same department**: after checking, members of the same department can also see and download this firmware

## 3. Other Operations

<img src="../../../../photo/docs/toolkits/firmware-other.png">

### 3.1 Modify Firmware

<img src="../../../../photo/docs/toolkits/firmware-update1.png">

<img src="../../../../photo/docs/toolkits/firmware-update.png" width="600" height="450">

### 3.2 Delete Firmware

<img src="../../../../photo/docs/toolkits/firmware-delete.png">

After deletion, the firmware no longer appears in the firmware list, and devices that have already been upgraded are not affected.

### 3.3 Download Firmware

<img src="../../../../photo/docs/toolkits/firmware-download.png">

### 3.4 Firmware Access Authorization

<img src="../../../../photo/docs/toolkits/firmware-access1.png">

<img src="../../../../photo/docs/toolkits/firmware-access.png" width="600" height="450">

By entering the email of a platform account, the platform account is automatically retrieved. Selecting the corresponding account can authorize firmware access to that account; the same is true for authorizing an organization.

Only the authorized account (and the members of the authorized organization) can see and use this firmware.

### 3.5 Firmware Redemption Code Generation

<img src="../../../../photo/docs/toolkits/firmware-code1.png">

<img src="../../../../photo/docs/toolkits/firmware-code.png" width="600" height="450">

Firmware redemption code generation is used for upgrading with OTA Assistant in the APP. For details, please refer to OTA Assistant on the APP page.
