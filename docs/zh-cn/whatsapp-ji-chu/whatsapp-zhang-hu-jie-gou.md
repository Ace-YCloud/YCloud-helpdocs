---
doc_id: doc_whatsapp_ji_chu_whatsapp_zhang_hu_jie_gou
language: zh-CN
title: "WhatsApp帐户结构"
slug: whatsapp-zhang-hu-jie-gou
path: whatsapp-ji-chu/whatsapp-zhang-hu-jie-gou
document_group: whatsapp-ji-chu
path_in_group: whatsapp-zhang-hu-jie-gou
parent_id: doc_whatsapp_ji_chu
order: 100
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T11:19:52.716Z
updated_at: 2026-04-02T11:19:52.716Z
last_synced_at: 2026-04-02T11:19:52.716Z
tags:
---

# WhatsApp帐户结构

## 帐户结构

要使用 WhatsApp 商业平台发送消息，您需要具备以下条件：

* Meta商业管理帐户（BM：Business Manager Account ）
* WhatsApp 商业帐户
* 电话号码

如果您满足所有这些要求，您可以开始通过 WhatsApp 商业平台向客户发送消息

<figure><img src="../.gitbook/assets/image (440).png" alt=""><figcaption><p>帐户结构</p></figcaption></figure>

## **BM帐户** <a href="#facebook-business-manager-account" id="facebook-business-manager-account"></a>

Meta商业管理帐户（BM：Business Manager Account ）这是 Meta 提供的管理工具，用于代表一家企业管理 Facebook、Instagram 和 WhatsApp 上的业务。

如果您还没有 BM帐户，可以访问[https://business.facebook.com/](https://business.facebook.com/)创建一个。

{% hint style="info" %}
您需要先拥有一个Facebook个人账户才可以创建BM帐户。
{% endhint %}

{% hint style="info" %}
建议：

* 在创建新的BM帐户之前，您需要与所有利益相关者核实公司是否存在已有的BM账户，以避免重复。&#x20;
* 将所有 Facebook 页面、Instagram 页面、广告帐户和WABA帐户关联到同一个BM帐户，避免信息丢失。同时，它将有助于提升WABA帐户的信任等级，不容易突然被封禁。
{% endhint %}



## WhatsApp 商业帐户 (WABA)

WhatsApp 商业帐户 (WABA) ，用于管理在 WhatsApp 商业平台中注册的电话号码。当您使用 YCloud 通过 WhatsApp 与您的最终用户联系时，我们将代表您创建和管理 WABA。&#x20;

每个 WABA 都有自己的 ID。

您可以在 BM帐户 中创建无限数量的 WABA，并且每个 YCloud 帐户可以与无限数量的 WABA 相关联。但WABA本身不能用于发送消息，您需要通过WABA中的电话号码收发消息。



## 电话号码

电话号码需要与 WhatsApp 帐户（WABA）关联，以便该帐户可以发送和接收消息。

电话号码是您选择发送 WhatsApp 消息的发件人，它与 WABA 相关联。

每个电话号码都有自己的显示名称，即在 WhatsApp 消息中向用户显示的品牌名称。

单个经过企业认证的 BM帐户 最多可包含 20 个不同的电话号码。此限制可根据请求（需要向YCloud团队提交工单）扩展至 120 个号码。如果是没有经过企业认证的 BM账户 ，您只能关联两个电话号码，每日发送信息次数限制为 250 次。

要将电话号码注册到WABA帐户内，您的企业电话号码必须满足以下条件：

* 您必须是该电话号码的所有者。
* 电话号码必须包含国家/地区代码，例如固定电话和手机号码。
* 该电话号码必须能够接听语音电话或短信。
* 该电话号码以前一定没有注册过WhatsApp（所有类型的账户）。

如果您想使用已在 WhatsApp App 或 WABA 上注册的电话号码，请参阅我们的迁移指南

* [将客户应用程序电话号码迁移至 WhatsApp Business 平台](https://developers.facebook.com/docs/whatsapp/on-premises/get-started/migrate-existing-whatsapp-number-to-a-business-account)
* 将电话号码迁移至其他 WABA



