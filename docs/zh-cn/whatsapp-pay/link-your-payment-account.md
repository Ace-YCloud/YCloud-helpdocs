---
doc_id: doc_whatsapp_pay_link_your_payment_account
language: zh-CN
title: "连接你的收款账户"
slug: link-your-payment-account
path: whatsapp-pay/link-your-payment-account
document_group: whatsapp-pay
path_in_group: link-your-payment-account
parent_id: doc_whatsapp_pay
order: 0
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T07:25:00.860Z
updated_at: 2026-04-02T07:25:00.860Z
last_synced_at: 2026-04-02T07:25:00.860Z
tags:
---

# 连接你的收款账户

YCloud正式支持了在WhatsApp中完成原生支付。不过，该功能目前仅对印度地区的企业和用户开放，且需要您连接指定的第三方支付软件：BillDesk, Razorpay, PayU 和 Zaakpay。

{% hint style="info" %}
请注意：以下步骤需要BM的管理员找第三方支付的管理员进行协作，才能完成全部的连接流程。
{% endhint %}

## 步骤1:

登陆您的BM账户，点击Payment configurations > New configuration

<figure><img src="../.gitbook/assets/image (807).png" alt=""><figcaption></figcaption></figure>

## 步骤2:

{% hint style="info" %}
配置您的收款方式，以下是Razorpay作为具体第三方支付账户的例子。
{% endhint %}

2.1 输入您配置的名称

<figure><img src="../.gitbook/assets/image (809).png" alt=""><figcaption></figcaption></figure>

2.2 连接配置和网关。在这一步，如果您是第三方支付账户的管理员，请选择Connect now; 如果您不是第三方支付账户的管理员，请选择 Account owner will connect later。

<figure><img src="../.gitbook/assets/企业微信截图_636f27d5-c217-4e5f-8f00-ce499cdc94b1.png" alt=""><figcaption></figcaption></figure>

2.3 输入第三方支付管理员的邮箱发送验证邮件，或者点击Copy link手动发送给第三方支付账户管理员进行验证，完成后点击Done。

<figure><img src="../.gitbook/assets/image (810).png" alt=""><figcaption></figcaption></figure>

2.4 当第三方支付管理员完成验证之后，状态会变为Needs Testing

<figure><img src="../.gitbook/assets/image (811).png" alt=""><figcaption></figcaption></figure>



## 步骤3：

复制链接并将链接发送到第三方支付账户管理员的邮箱。管理员点开链接后，会跳转到授权页面，点击Authorize完成授权。

<figure><img src="../.gitbook/assets/image (812).png" alt=""><figcaption></figcaption></figure>

## 步骤4:

4.1 完成授权后，状态会显示Need Testing。这时候，BM账户管理员需要测试连接是否成功。测试成功后，状态会变成Active。当状态变为Active后，整个连接过程就完成了。

<figure><img src="../.gitbook/assets/image (187).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (188).png" alt=""><figcaption></figcaption></figure>



