---
doc_id: doc_integrations_integrate_with_n8n_index
language: zh-CN
title: "通过n8n集成"
slug: index
path: integrations/integrate_with_n8n/index
document_group: integrations
path_in_group: integrate_with_n8n/index
parent_id: doc_integrations_integrate_with_n8n
order: 0
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T07:26:41.101Z
updated_at: 2026-04-02T07:26:41.101Z
last_synced_at: 2026-04-02T07:26:41.101Z
tags:
---

# 通过n8n集成

### 概述

YCloud 支持通过 n8n 进行自动化集成。

n8n 是一款开源的可视化工作流自动化平台，可用于将 YCloud Webhook、API 事件与第三方系统（如 CRM、数据库、AI 服务等）进行灵活连接。

在 YCloud 的典型使用场景中，n8n 常用于：

* 接收 YCloud Webhook 事件
* 对消息或用户行为进行条件判断与处理
* 调用 AI / 外部 API 进行分析
* 将结果同步至 CRM、内部系统或数据仓库

***

### 使用前准备

在开始之前，请确保已具备以下条件：

* 已部署并可访问的 n8n 实例
* 已获取 n8n 的登录账号与权限
* 如需调用大模型或第三方 API，请提前准备对应的 API Key

***

### n8n 官方文档

关于 n8n 的安装、基础概念与使用方式，请直接参考 n8n 官方文档：

👉 [https://docs.n8n.io](https://docs.n8n.io/)

以下内容在官方文档中已有完整说明：

* Workflow（工作流）与 Node（节点）的基本概念
* Webhook Trigger 的配置方式
* Expression（表达式）语法
* Credentials（凭证）管理
* Execution（执行记录）与调试方法

***

### 与 YCloud 的集成方式

在 YCloud 中，可将 Webhook 地址 配置为 n8n 的 Webhook URL，使 n8n 成为事件处理的中间层。

### 说明

* **n8n 为第三方工具，YCloud 不对其功能本身提供维护或支持**
* 建议在 n8n 中区分 测试环境（Test URL） 与 生产环境（Production URL）
* 请妥善管理 API Key、Webhook 地址等敏感信息
