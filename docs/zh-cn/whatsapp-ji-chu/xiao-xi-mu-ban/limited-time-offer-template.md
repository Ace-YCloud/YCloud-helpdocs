---
doc_id: doc_whatsapp_ji_chu_xiao_xi_mu_ban_limited_time_offer_template
language: zh-CN
title: "限时优惠模板"
slug: limited-time-offer-template
path: whatsapp-ji-chu/xiao-xi-mu-ban/limited-time-offer-template
document_group: whatsapp-ji-chu
path_in_group: xiao-xi-mu-ban/limited-time-offer-template
parent_id: doc_whatsapp_ji_chu_xiao_xi_mu_ban
order: 50
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

# 限时优惠模板

限时优惠模板可让您在模板消息中显示优惠代码的到期日期和正在运行的倒计时器，让您轻松传达限时优惠并推动客户参与。限时优惠模版仅适用于营销模版消息。

<figure><img src="../../.gitbook/assets/image (550).png" alt="" width="363"><figcaption></figcaption></figure>

### 限时优惠组件 <a href="#limitations" id="limitations"></a>

限时优惠模版由标题、限时优惠组件、正文和按钮组成。限时优惠组件包含限时优惠标题、限时优惠时间和限时优惠码，规则如下：

* 标题为必填。
* 限时优惠组件默认开启，您可以手动关闭。若限时优惠组件开启，您可以在发送这个模版的时候上传优惠的具体有效期。⚠️ 创建限时优惠模版的时候不需要上传具体有效期。
* 若您选择添加“复制优惠码（Copy Code）”按钮，并且填写了示例优惠码，则会显示优惠码；否则，不显示优惠码。
* 访问网站按钮为必填，复制优惠码为选填。



#### 展示效果说明

以下效果以 WhatsApp 移动端的实际展示为例。\
使用 WhatsApp 网页应用程序或桌面应用程序查看限时优惠模板消息时，用户不会直接看到限时优惠组件的展示效果，而会看到一条提示消息，表明他们已收到一条消息。

**1. 未设置有效期**

如果发送消息时未设置有效期，限时优惠组件不会显示具体截止时间，也不会显示 `Offer ended` 状态。\
如果模板中配置了“复制优惠码（Copy Code）”按钮，并填写了优惠码，用户仍可看到优惠码并复制优惠码。

**2. 设置有效期后，优惠未过期时**

如果发送消息时设置了有效期，且优惠仍在有效期内，限时优惠组件会显示截止时间和优惠码。\
如果模板中配置了“复制优惠码（Copy Code）”按钮，用户可以直接复制优惠码。

<figure><img src="../../.gitbook/assets/limited-time offer-demo-2.png" alt="" width="156"><figcaption></figcaption></figure>

**3. 设置有效期后，优惠已过期时**

如果优惠已超过设置的有效期，限时优惠组件会显示 `Offer ended`。\
同时，“复制优惠码（Copy Code）”按钮会消失，用户无法再复制优惠码。

<figure><img src="../../.gitbook/assets/limited-time-offer-demo-3-expired.png" alt="" width="188"><figcaption></figcaption></figure>

### 创建限时优惠模版

您可以在YCloud的模版里创建限时优惠模版。

首先，在在营销模版目录下选择限时优惠模版。

<figure><img src="../../.gitbook/assets/image (870).png" alt=""><figcaption></figcaption></figure>

然后，依次填充标题、限时优惠组件、正文和按钮。

<figure><img src="../../.gitbook/assets/image (872).png" alt=""><figcaption></figcaption></figure>

⚠️ 使用 WhatsApp 网页应用程序或桌面应用程序查看限时优惠模板消息的用户将看不到该优惠，但会看到一条消息，表明他们已收到一条消息。

💡模板审核通过后，您可以使用 3 种方式发送此模板消息：

1. [Inbox：发送给某1个联系人](../../inbox/fa-qi-xin-liao-tian.md)
2. [Campaign：群发广播](../../campaign/chuang-jian-whatsapp-ying-xiao-huo-dong.md#bu-zhou-2-fa-song-ying-xiao-xiao-xi)
3. [通过 API 发送](https://docs.ycloud.com/reference/whatsapp_message-send-directly)

