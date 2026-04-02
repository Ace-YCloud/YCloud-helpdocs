---
doc_id: doc_ctwa_click_to_whatsapp_ad_tiktok_messaging_ad
language: zh-CN
title: "TikTok 消息广告"
slug: tiktok-messaging-ad
path: ctwa-click-to-whatsapp-ad/tiktok-messaging-ad
document_group: ctwa-click-to-whatsapp-ad
path_in_group: tiktok-messaging-ad
parent_id: doc_ctwa_click_to_whatsapp_ad
order: 720
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T11:05:49.073Z
updated_at: 2026-04-02T11:05:49.073Z
last_synced_at: 2026-04-02T11:05:49.073Z
tags:
---

# TikTok 消息广告

### 概述

按本篇指引完成配置后，您可以实现：\
在 TikTok 投放跳转到 WhatsApp 的即时消息广告，将广告流量直接引导至 WhatsApp 对话，并通过 YCloud Inbox 统一承接和跟进潜在客户会话。

下文将依次介绍:前期准备、广告账户授权、WhatsApp Business 号码绑定、广告创建，以及追踪与转化设置。



### 什么是 TikTok 消息广告？

TikTok 消息广告是一种帮助企业通过广告与潜在客户发起对话的广告形式。根据会话发起方式的不同，通常可以分为两类：

* 用户点击广告后，在 TikTok 内直接与商家开始对话。
* 用户点击广告后，跳转到第三方消息应用继续沟通，例如 WhatsApp。

YCloud 当前支持的是第二种，即跳转到 WhatsApp 的即时消息广告。

### 为什么选择 TikTok 消息广告？

对于以咨询、留资和销售转化为目标的业务来说，TikTok 消息广告可以提供更直接的客户沟通路径。与“广告点击后进入落地页，再提交表单”的方式相比，这种广告形式更适合需要快速响应客户咨询的场景，主要体现在以下几个方面：

* 将广告流量直接引导至 WhatsApp，对话路径更短。
* 用户发起咨询后，可由 YCloud Inbox 统一承接和跟进。
* 结合会话事件和转化回传，有助于持续优化广告投放效果。

### 实际投放效果示意

下图演示了用户在 TikTok 中看到广告，在点击 CTA 后跳转到 WhatsApp 发起会话的实际效果。

<figure><img src="../../.gitbook/assets/tiktok-ctwa-demo (1).gif" alt=""><figcaption></figcaption></figure>



### 客户前期准备工作

开始配置前，建议先确认 TikTok、WhatsApp 和 YCloud 相关资源已经准备完成，以减少授权失败、号码选择错误或后续事件无法回传等问题。

#### 配置流程总览

下图展示

您在 YCloud 和 TikTok Ads Manager 分别需要完成的操作，以及这些操作的前后顺序。

<figure><img src="../../.gitbook/assets/YCloud-tiktok connected flow.png" alt=""><figcaption></figcaption></figure>

#### TikTok 侧准备

* 已确认本次投放将使用的 TikTok Ad Account，且该账户可正常使用。
* 当前操作人对目标 TikTok Ad Account 拥有足够权限，并可完成授权操作。

#### WhatsApp 侧准备

* 已有接入 YCloud 的 WhatsApp Business 号码。
* 该号码将用于承接 TikTok 广告带来的用户咨询。
* 已确认对应团队可以及时处理进入 WhatsApp 的潜在客户会话。

#### YCloud 侧准备

* 已开通并可正常登录 YCloud。
* 用于投放的 WhatsApp Business 号码已在YCloud后台 完成绑定,如下图：

<figure><img src="../../.gitbook/assets/WHATSAPP_ACCOUNT-CONNECTED (1).png" alt=""><figcaption></figcaption></figure>

* 如果您尚未绑定，请先点此：[添加WhatsApp 商业号码](https://helpdocs.ycloud.com/help-center/zh/whatsapp-accounts-zhang-hao-guan-li/chuang-jian-whatsapp-api-zhang-hao/tong-guo-qian-ru-shi-zhu-ce-chuang-jian-waba)。



### 操作步骤

1. 步骤1、2：在YCloud后台配置：[链接广告账户](tiktok-ad-introduction.md)、[绑定WhatsApp号码](tiktok-ad-introduction.md)
2. 步骤3、4、5：[在TikTok 广告后台 创建TikTok 消息广告](create-tiktok-instant-messaging-ad.md)；
3. 步骤6、7、8：[YCloud承接广告流量、广告追踪&转化](tiktok-ad-traffic-delivery-tracking-and-conversion.md)

