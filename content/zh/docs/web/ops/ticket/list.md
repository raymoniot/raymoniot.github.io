---
title: 工单列表
description: 所有工单的概况列表，可以进行工单状态变更、工单修改和评分，并区分我发起的、待办、与我相关
weight: 3
---

# 功能概述

工单列表展示所有工单，并按与当前账号的关系分成几个标签页：

- **我发起的**：当前账号创建的工单
- **待办**：需要当前账号处理的工单
- **与我相关**：当前账号参与过的工单（如被回复或被抄送）
- **全部**：当前账号数据权限内的所有工单

<img src="/../../zh/photo/docs/ops/ticket/ticket-list.png">

列表中的信息包括工单编号、主题、工单类型、在手人（或发起人）、首次响应截止、关闭截止、优先级、状态和操作。上方的「快捷查找」可以按关键词快速定位工单。

## 1.工单状态变更

<img src="/../../zh/photo/docs/ops/ticket/ticket-status.png">

工单处理过程中需要及时更新状态，状态分为：

- **打开**：工单已建立，等待处理
- **待定**：需要等待用户确认或补充信息
- **已解决**：问题已处理完成
- **已关闭**：工单结束

## 2.工单修改

<img src="/../../zh/photo/docs/ops/ticket/ticket-update.png">

<img src="/../../zh/photo/docs/ops/ticket/ticket-update1.png">

## 3.待办

<img src="/../../zh/photo/docs/ops/ticket/ticket-undeal.png">

待办中的工单会显示优先级（高、中、低），可以按优先级先处理紧急的问题。

## 4.与我相关

<img src="/../../zh/photo/docs/ops/ticket/ticket-me.png">

## 5.工单评分

工单解决后可以对处理结果评分（正面、中立、负面），评分结果会统计到[工单看板]({{< ref "dashboard" >}} "工单看板")的评分板块。
