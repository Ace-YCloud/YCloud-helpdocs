---
doc_id: doc_calling_overview
language: zh-CN
title: "WhatsApp Calling 简介"
slug: overview
path: calling/overview
document_group: calling
path_in_group: overview
parent_id: doc_calling
order: 450
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T11:10:44.061Z
updated_at: 2026-04-02T11:10:44.061Z
last_synced_at: 2026-04-02T11:10:44.061Z
tags:
---

# WhatsApp Calling 简介

WhatsApp Calling 是 WhatsApp Business Cloud API 提供的一项语音通话（VoIP）能力，让企业能够在 WhatsApp 内与客户进行实时语音沟通。

当前支持两类通话方式：

* 呼入通话：客户主动拨打给企业
* 呼出通话：企业主动拨打给客户



## 计费方式

#### 呼入通话

* 免费 —— 无论企业是否接听，均不产生费用。

#### 呼出通话

* 根据实际 接通时长 收费
* 计费单位：每 6 秒为 1 个计费单位（不足 6 秒按 6 秒计费）
* 费用根据用户 手机号码的国家代码 而定

举例：

印尼价格为 0.0242 USD / 分钟

若企业向印尼用户外呼并在第9 秒挂断：

→ 计费 = 2 个单位 × 0.0242/10 USD = 0.00484 USD

👉 [_点击查看各国详细价格_](https://www.ycloud.com/pricing#price-table)





## 用户发起呼叫（呼入）

用户可通过以下 3 种方式向企业发起语音通话：

#### 1. 在 WhatsApp 会话窗口顶部展示呼叫按钮

开启后，客户可直接点击 “Call” 按钮拨打企业号码。

<figure><img src="../.gitbook/assets/image (873).png" alt=""><figcaption></figcaption></figure>

#### 2.呼入链接（Call-in Link）

企业可生成呼入链接并放置在网站、邮件或 WhatsApp 消息中。

用户点击即可发起语音通话。

<figure><img src="../.gitbook/assets/image (874).png" alt=""><figcaption></figcaption></figure>



#### 3. 消息内加入呼入按钮

在消息模板或互动消息中加入 “Call In” 按钮，引导用户快速拨打。

<figure><img src="../.gitbook/assets/image (875).png" alt=""><figcaption></figcaption></figure>

##

## 企业发起呼叫（外呼）

使用 WhatsApp 外呼前，您的商业账号需满足以下条件：

1. BM 消息额度（message limit）达到 2000 级
2. 商业号码的注册区号 不属于以下国家／地区：
   * 美国（+1）
   * 加拿大（+1）
   * 土耳其（+90）
   * 埃及（+20）
   * 越南（+84）
   * 尼日利亚（+234）



为保护用户隐私，企业在主动外呼前必须先获得用户授权。

可通过以下消息方式向客户请求通话授权：

* 携带 calling request 的模板消息
* 带按钮的互动消息

客户收到后可选择 “允许” 或 “拒绝”。客户允许后，企业可在授权有效期内发起外呼。

消息示例：

<figure><img src="../.gitbook/assets/image (876).png" alt=""><figcaption></figcaption></figure>

##

## 如何开始使用 WhatsApp Calling？

YCloud 提供两种接入方式（只能二选一）：

#### 1. HTTPS API 接入

若您计划通过 API 实现呼入／呼出功能，请联系我们开通 Calling 功能。

可参考 API 文档链接，[👉点击访问](https://docs.ycloud.com/reference/whatsapp-calling-examples)

#### 2. 通过 YCloud 平台内直接使用（推荐）

以下为基于 YCloud 平台的完整使用教程。





## 在 YCloud 中开启 WhatsApp Calling 功能

每个商业号码都可以独立开启或关闭 Calling 功能。

路径：WhatsApp accounts → 号码设置 → Calling<br>

打开开关即可开始使用。

<figure><img src="../.gitbook/assets/image (877).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (878).png" alt=""><figcaption></figcaption></figure>

##

## 在商业号码上展示呼入按钮

勾选 Call Icon visibility，即可在号码详情页右侧显示呼叫按钮。

客户可直接点击进行呼入。

<figure><img src="../.gitbook/assets/image (879).png" alt=""><figcaption></figcaption></figure>

##

## 配置外呼权限

您可以为团队成员分配可外呼的商业号码。仅授权的成员才可在 YCloud 平台上使用该号码发起外呼。

> 提示：此限制仅适用于 YCloud 平台 UI 的外呼功能。 若通过 API 发起 WhatsApp 通话，则不受此限制。

<figure><img src="../.gitbook/assets/image (880).png" alt=""><figcaption></figcaption></figure>
