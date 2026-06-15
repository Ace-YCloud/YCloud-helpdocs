---
doc_id: doc_integrations_you_hui_quan_you_hui_quan_gong_ju_shi_yong
language: zh-CN
title: "优惠券工具使用"
slug: you-hui-quan-gong-ju-shi-yong
path: integrations/you-hui-quan/you-hui-quan-gong-ju-shi-yong
document_group: integrations
path_in_group: you-hui-quan/you-hui-quan-gong-ju-shi-yong
parent_id: doc_integrations_you_hui_quan
order: 0
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T07:26:57.008Z
updated_at: 2026-04-02T07:26:57.008Z
last_synced_at: 2026-04-02T07:26:57.008Z
tags:
---

# 优惠券工具使用

管理企业的优惠活动。企业可以上传自己的优惠券码，并限制每个客户只能领取1个优惠券码。上传后的优惠码可在ChatBot、Inbox、Campaign中进行分发。

## 使用场景

扫码领取优惠券，客户通过二维码到您的商业账号中领取优惠券。



## 教程

### 步骤1：创建优惠券活动

#### 步骤1.1：开通优惠券功能

入口：[Integrations](https://www.ycloud.com/console/#/app/integrations/all)，点击Install按钮开通

<figure><img src="../../.gitbook/assets/image (704).png" alt=""><figcaption></figcaption></figure>

#### 步骤1.2: 创建优惠券活动

从左侧导航Integrations>[Coupons](https://www.ycloud.com/console/#/app/integrations/coupon/list)进入优惠券页面

点击【+ New Coupons】&#x20;

<figure><img src="../../.gitbook/assets/image (705).png" alt=""><figcaption></figcaption></figure>

#### 步骤1.3：配置活动信息

* 优惠券类型：Code类型（优惠码）。暂是仅支持这一种类型，有其他类型需求可联系我们沟通。
* 活动名称：优惠券活动名称
* 活动备注：活动备注信息，非必填。
* 领取限制：每人仅支持领取1次。
* 活动持续时间：活动时间设置。在活动时间范围外停止发送优惠券。

信息确认无误后点击 提交。

<figure><img src="../../.gitbook/assets/image (706).png" alt=""><figcaption></figcaption></figure>

#### 步骤1.4：上传优惠券Code

点击上传按钮

<figure><img src="../../.gitbook/assets/image (707).png" alt=""><figcaption></figcaption></figure>

上传优惠码 表格。可点击模板按钮进行模板下载。

{% hint style="info" %}
注意：上传的Excel表格，Code必须在第一列。YCloud会自动去重重复的优惠码。
{% endhint %}

<figure><img src="../../.gitbook/assets/image (708).png" alt=""><figcaption></figcaption></figure>

上传完成后点击保存

<figure><img src="../../.gitbook/assets/image (709).png" alt=""><figcaption></figcaption></figure>

### 步骤2：在Chatbot中配置领取流程

#### 步骤2.1：创建Chatbot

若您已经有Chatbot，可直接进入现成的Chatbot，若还未配置过，可查看[创建一个Chatbot](../../chatbot/chuang-jian-yi-ge-chatbot.md)教程。

#### 步骤2.2：创建Flow

选择需要配置的Chatbot，点击创建Flow按钮。

<figure><img src="../../.gitbook/assets/image (711).png" alt=""><figcaption></figcaption></figure>

#### 步骤2.3：配置Flow keyword

Keyword设置为领取的关键词。

举例：若您希望客户在命中“**领取新人优惠券**”时进行优惠券分发，可把Keyword设置为**领取新人优惠券。**

<figure><img src="../../.gitbook/assets/image (710).png" alt=""><figcaption></figcaption></figure>

#### 步骤2.4：配置发送的优惠券

在Flow中增加Send message 组件

<figure><img src="../../.gitbook/assets/image (222).png" alt=""><figcaption></figcaption></figure>

在消息中点击优惠券变量，选择要插入的优惠券活动。

<figure><img src="../../.gitbook/assets/image (223).png" alt=""><figcaption></figcaption></figure>

编辑成功后，链接Keyword和Send message组件。完成后保存Flow

<figure><img src="../../.gitbook/assets/image (225).png" alt=""><figcaption></figcaption></figure>

### 步骤3：生成二维码分享（非必选，仅扫码领券场景配置)

给号码生成一个二维码，设置关键词为：**领取新人优惠券**。[查看详细的聊天链接配置教程](../../whatsapp-accounts-zhang-hao-guan-li/shou-ji-hao-ma-guan-li/liao-tian-lian-jie.md)

<figure><img src="../../.gitbook/assets/image (227).png" alt=""><figcaption></figcaption></figure>
