---
doc_id: doc_whatsapp_ji_chu_xiao_xi_mu_ban_shen_fen_yan_zheng_xiao_xi_mu_ban
language: zh-CN
title: "身份验证消息模板"
slug: shen-fen-yan-zheng-xiao-xi-mu-ban
path: whatsapp-ji-chu/xiao-xi-mu-ban/shen-fen-yan-zheng-xiao-xi-mu-ban
document_group: whatsapp-ji-chu
path_in_group: xiao-xi-mu-ban/shen-fen-yan-zheng-xiao-xi-mu-ban
parent_id: doc_whatsapp_ji_chu_xiao_xi_mu_ban
order: 10
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

# 身份验证消息模板

<figure><img src="../../../.gitbook/assets/image (438).png" alt="" width="563"><figcaption></figcaption></figure>

带有 OTP 按钮的身份验证模板由以下内容组成：

* 预设认证消息模板固定文本：
  * \<VERIFICATION\_CODE> 是您的验证码。
  * 安全免责声明（可选）：为了您的安全，请勿共享此代码。
  * 过期警告（可选）：此代码将在 \<NUM\_MINUTES> 分钟后过期。
  * 按钮：复制代码或一键自动填充按钮。
  * 消息有效期：如果消息没有在有效期范围内送达，您将不会被收取费用，您的客户将不会看到该消息。

代码长度不能超过 15 个字符。不支持 URL、媒体和表情符号。由于带有 OTP 按钮的身份验证模板仅由预设文本和按钮组成，因此其被暂停的风险大大降低。



## 复制代码身份验证模板 <a href="#copy-code-authentication-templates" id="copy-code-authentication-templates"></a>

复制代码身份验证模板允许您向用户发送一次性密码或代码以及复制代码按钮。

![](https://scontent-hkg1-2.xx.fbcdn.net/v/t39.2365-6/391709210_6733218460105388_4204949555628827374_n.png?stp=dst-webp&_nc_cat=107\&ccb=1-7&_nc_sid=e280be&_nc_ohc=krz-7v4xBIQQ7kNvgHdqrBW&_nc_ht=scontent-hkg1-2.xx\&oh=00_AYDAQ1dzpZiwvWmGy67v_uYh4zI5iqD1BdIyD24xn0pc6g\&oe=6694D0BD)

当 WhatsApp 用户点击复制代码按钮时，WhatsApp 客户端会将密码或代码复制到设备的剪贴板。然后，用户可以切换到您的应用并将密码或代码粘贴到您的应用中。

请参阅[复制代码身份验证模板](fu-zhi-yan-zheng-ma-shen-fen-yan-zheng-mu-ban.md)以了解如何使用它们。



## 一键自动填充身份验证模板 <a href="#one-tap-autofill-authentication-templates" id="one-tap-autofill-authentication-templates"></a>

身份验证模板包括一键自动填充按钮。

![](https://scontent-hkg1-2.xx.fbcdn.net/v/t39.2365-6/393789031_872892117564016_6400271480127333734_n.png?stp=dst-webp&_nc_cat=104\&ccb=1-7&_nc_sid=e280be&_nc_ohc=YQvdnWWnjhYQ7kNvgF-Fdpy&_nc_ht=scontent-hkg1-2.xx\&oh=00_AYBD2XbjW4aCaL2vLfdKi2ym247Lt4J9K9Ha07LQ29ZmlA\&oe=6694C268)

当 WhatsApp 用户点击自动填充按钮时，WhatsApp 客户端会触发一项活动，打开您的应用程序并向其提供密码或代码。

请参阅[一键自动填充身份验证模板](yi-jian-zi-dong-tian-chong-shen-fen-yan-zheng-mu-ban.md)以了解如何使用它们。



## 零点击身份验证模板 <a href="#zero-tap-authentication-templates" id="zero-tap-authentication-templates"></a>

零点击身份验证模板允许您的用户通过 WhatsApp 接收一次性密码或代码，而无需离开您的应用程序。

<figure><img src="../../../.gitbook/assets/image (531).png" alt="" width="375"><figcaption></figcaption></figure>

当您应用中的用户请求密码或代码并且您使用零点击身份验证模板提供该密码或代码时，WhatsApp 客户端会广播所包含的密码或代码，然后您的应用可以使用广播接收器捕获该密码或代码。

请参阅[零点击身份验证模板](ling-dian-ji-shen-fen-yan-zheng-mu-ban.md)来了解如何使用它们。



## **最佳实践**

* 在向用户的 WhatsApp 电话号码发送一次性密码或代码之前，请先确认该号码。
* 向用户明确说明密码或代码将发送到他们的 WhatsApp 电话号码，尤其是当您为用户提供多种接收密码或代码的方式时。请参阅[获取选择加入](https://developers.facebook.com/docs/whatsapp/overview/getting-opt-in)以获取更多提示。
* 当用户将密码或代码粘贴到您的应用中，或者您的应用通过一键自动填充按钮流程接收该密码或代码时，请向用户明确表明您的应用已捕获该密码或代码。



##

&#x20;
