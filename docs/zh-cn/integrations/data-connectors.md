---
doc_id: doc_integrations_data_connectors
language: zh-CN
title: "数据连接器"
slug: data-connectors
path: integrations/data-connectors
document_group: integrations
path_in_group: data-connectors
parent_id: doc_integrations
order: 0
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T07:26:18.120Z
updated_at: 2026-04-02T07:26:18.120Z
last_synced_at: 2026-04-02T07:26:18.120Z
tags:
---

# 数据连接器

## 数据连接器是什么？

数据连接器是深度嵌入的集成工具，可将您的实时外部数据接入平台。 您可以从那些需要团队成员需要花费大量时间回答，而答案所涉及的信息目前在我们的平台上又暂时还无法获取的问题开始着手。

这些问题可能仅仅需要一些外部的数据辅助即可解决，例如“我的订单是否已送达？”或者是在您的外部系统中更新信息，例如“重新安排配送”或“处理退款”。

## 创建数据连接器

首先，通过左侧菜单的集成>数据连接器访问该功能。

<figure><img src="../.gitbook/assets/image (61).png" alt=""><figcaption></figcaption></figure>

在这里，您可以设置数据连接器来连接外部数据。您可以通过点击\[+新建数据连接器]按钮来创建一个。您还可以按名称和状态搜索特定的数据连接器。

<figure><img src="../.gitbook/assets/image (62).png" alt=""><figcaption></figcaption></figure>

## 名称和描述

为你的数据连接器取一个能清晰表明其特定功能的名称（例如，“retrieve\_order\_id”）。在描述字段中，描述何时使用此连接器以及它将获取哪些数据（例如，“获取提供的订单 ID 的订单详情”）。

<figure><img src="../.gitbook/assets/image (63).png" alt=""><figcaption></figcaption></figure>

## API 链接

### API 请求

接下来，填写请求详情。在这里，您需要输入要连接的第三方系统的 HTTPS URL。您可以定义具体的请求方式：

* **GET** - 从第三方系统读取并存储信息。
* **POST** - 创建或向第三方系统添加信息。
* **PUT** - 更新第三方系统中的信息。
* **DELETE** - 从第三方系统中移除信息。
* **PATCH** - 更新第三方系统中的信息。

<figure><img src="../.gitbook/assets/image (64).png" alt=""><figcaption></figcaption></figure>

### API headers

您可以通过点击+Add header来选择向此请求添加任何额外参数，然后输入**键值对：**

<figure><img src="../.gitbook/assets/image (65).png" alt=""><figcaption></figcaption></figure>

### 请求体

如果您正在发起 POST 或 PUT 请求，您将可以选择提供请求体，以包含您希望在请求中发送的任何数据：

<figure><img src="../.gitbook/assets/image (66).png" alt=""><figcaption></figcaption></figure>

## 测试响应

接下来，你需要测试此数据连接器的响应，以确保它从你连接的外部系统中获取到了正确的数据。

{% hint style="warning" %}
**重要提示：**&#x6D4B;试此请求会与 API 建立连接，因此它将完成你创建的数据连接器。例如，如果你要求它从 API 删除数据，此信息将被删除。尝试使用 GET 请求进行测试，以确保你只是读取信息而不更改它。
{% endhint %}

点击**测试请求**以检查数据连接器是否已正确配置。

<figure><img src="../.gitbook/assets/image (67).png" alt=""><figcaption></figcaption></figure>

## 激活

一旦测试没有问题，你的数据连接器即可投入使用。点击右上角Set live 进行激活。

<figure><img src="../.gitbook/assets/image (68).png" alt=""><figcaption></figcaption></figure>

## 设置为草稿

如果您想弃用不再需要的旧数据连接器，可以将它们切换为草稿状态。

您可以点击想要移至草稿状态的数据连接器，然后选择“设为草稿”，或在列表中关闭状态开关。

<figure><img src="../.gitbook/assets/image (970).png" alt=""><figcaption></figcaption></figure>

这将检查此数据连接器的所有依赖项。在将其移至草稿状态之前，您需要审查并解决这些依赖项。
