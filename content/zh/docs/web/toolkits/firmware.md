---
title: 固件管理
description: 设备OTA固件管理：按设备类型维护固件，支持固件搜索、新增固件、修改固件、下载固件、访问授权、生成兑换码
weight: 1
---

# 功能概述

平台设备固件管理，包含固件搜索、新增固件、修改固件、下载固件、访问授权、生成兑换码等

<img src="/../../zh/photo/docs/toolkits/firmware-enter.png">

固件按设备类型（采集器、逆变器、电池系统、电池 PACK、微逆等）分开维护，列表显示固件名称、固件版本、扩展信息、备注、文件大小和更新时间。远程交互和设备详情页做固件升级时，只会看到当前账号有权限且与目标设备类型匹配的固件。

## 1.固件搜索

<img src="/../../zh/photo/docs/toolkits/firmware-search1.png">

<img src="/../../zh/photo/docs/toolkits/firmware-search.png" width="700" height="550">

可以根据设备类型或固件名称进行高级搜索

## 2.新增固件

<img src="/../../zh/photo/docs/toolkits/firmware-add.png">

<img src="/../../zh/photo/docs/toolkits/firmware-add1.png" width="600" height="450">

- **设备类型**：必填，按设备类型/品牌/型号三级选择，固件只能用于所选的型号
- **固件名称、固件版本**：必填，**固件版本**不易过长
- **扩展信息**：用于区分同一型号下的固件差异（例如是否区分序列芯片）
- **固件文件**：必填，文件大小不能超过 2MB，请确保**固件文件合法**，否则将无法新增
- **授权给同部门成员**：勾选后同部门成员也可以看到并下载该固件

## 3.其他操作

<img src="/../../zh/photo/docs/toolkits/firmware-other.png">

### 3.1修改固件

<img src="/../../zh/photo/docs/toolkits/firmware-update1.png">

<img src="/../../zh/photo/docs/toolkits/firmware-update.png" width="600" height="450">

### 3.2删除固件

<img src="/../../zh/photo/docs/toolkits/firmware-delete.png">

删除后该固件不再出现在固件列表中，已经升级过的设备不受影响。

### 3.3下载固件

<img src="/../../zh/photo/docs/toolkits/firmware-download.png">

### 3.4固件访问授权

<img src="/../../zh/photo/docs/toolkits/firmware-access1.png">

<img src="/../../zh/photo/docs/toolkits/firmware-access.png" width="600" height="450">

通过输入平台账号的邮箱会自动检索平台账号，选择对应的账号可以将固件访问授权到该账号下，授权组织同理

只有被授权的账号（以及授权组织的成员）才能看到并使用这个固件。

### 3.5固件兑换码生成

<img src="/../../zh/photo/docs/toolkits/firmware-code1.png">

<img src="/../../zh/photo/docs/toolkits/firmware-code.png" width="600" height="450">

固件兑换码生成用于APP中使用OTA助手进行升级，详请参考APP页面OTA助手
