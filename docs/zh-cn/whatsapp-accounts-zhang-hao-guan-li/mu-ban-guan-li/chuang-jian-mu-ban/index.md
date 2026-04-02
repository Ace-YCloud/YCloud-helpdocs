---
doc_id: doc_whatsapp_accounts_zhang_hao_guan_li_mu_ban_guan_li_chuang_jian_mu_ban
language: zh-CN
title: "创建模板"
slug: chuang-jian-mu-ban
path: whatsapp-accounts-zhang-hao-guan-li/mu-ban-guan-li/chuang-jian-mu-ban
document_group: whatsapp-accounts-zhang-hao-guan-li
path_in_group: mu-ban-guan-li/chuang-jian-mu-ban
parent_id: doc_whatsapp_accounts_zhang_hao_guan_li_mu_ban_guan_li
order: 10
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T11:07:53.930Z
updated_at: 2026-04-02T11:07:53.930Z
last_synced_at: 2026-04-02T11:07:53.930Z
tags:
---

# 创建模板

## 创建营销、通知模板教程

### 步骤1：进入模板页面

1. 从左侧导航的 Templates中进入。账号内有多个WABA的用户请注意切换右上角的WABA空间。

<figure><img src="../../../.gitbook/assets/image (279).png" alt=""><figcaption><p>Templates</p></figcaption></figure>

2. 从WhatsApp accounts 中进入Templates。

<figure><img src="../../../.gitbook/assets/image (280).png" alt=""><figcaption><p>WABA>Templates</p></figcaption></figure>

### 步骤2：命名 & 选择模板类型

1. Template name: 模板名称。名称仅支持数字、小写字母和下划线\_。

{% hint style="info" %}
注意：名称是唯一的，也是在接口发送时调用的名称。
{% endhint %}

2. Category： 模板类型。模板有3种类型，根据模板内容进行选择：
   1. Utility：事务性模板。用于发送通知类的消息。
   2. Marketing：营销模板。所有带有营销意味的消息，以及所有打招呼类的消息。
   3. Authentication：验证码模板。固定内容，仅支持发送验证码。

<figure><img src="../../../.gitbook/assets/image (283).png" alt=""><figcaption><p>Template name &#x26; Category</p></figcaption></figure>

### 步骤3：选择语言

一种模板内容可以选择多种语言进行配置。点击Add lanuage可继续添加。

可将多个语言一起编辑完成后进行提交。

<figure><img src="../../../.gitbook/assets/image (282).png" alt=""><figcaption><p>Choose language</p></figcaption></figure>

点击语言右侧的Edit按钮可编辑删除语言。

<figure><img src="../../../.gitbook/assets/image (284).png" alt=""><figcaption><p>Edit language</p></figcaption></figure>

### 步骤4：编辑模板内容

[查看验证码模板创建介绍](https://helpdocs.ycloud.com/help-center/zh/whatsapp-accounts-zhang-hao-guan-li/mu-ban-guan-li/chuang-jian-mu-ban#yan-zheng-ma-mu-ban-chuang-jian-jie-shao)

以**营销**和**通知模板**内容为例：

1. Header（非必填）：Header类型支持：文字、图片、视频、文件。
2. Body（必填）：文字内容。支持emoji、加粗等文字样式。
3. Footer(非必填）：文本页脚。
4. Button（非必填）
   1. 最多可以添加10个Button
   2. Button类型有：
      1. Quick reply（快捷回复按钮）
      2. Visit website（页面跳转）
      3. Call phone number（打电话）
      4. Copy offer code（复制代码）
5. Variables：变量。变量可添加在Header, Body 或者 Visit website 中。添加变量时必须添加Sample，用于审核人员在审核时判断整个模板的发送内容。Sample仅用于审核，实际下发时必须传送变量值。

<figure><img src="../../../.gitbook/assets/image (89).png" alt=""><figcaption></figcaption></figure>

详细的模板内容可查看[消息模板](../../../whatsapp-ji-chu/xiao-xi-mu-ban/)文档

<figure><img src="../../../.gitbook/assets/image (107).png" alt=""><figcaption><p>Edit template</p></figcaption></figure>

### 步骤5：提交模板

所有语言编辑完成后，可滚至页面最下方点击提交按钮。

<figure><img src="../../../.gitbook/assets/image (108).png" alt=""><figcaption><p>Submit template</p></figcaption></figure>

确认提交模板内容无误后点击Confirm。

<figure><img src="../../../.gitbook/assets/image (109).png" alt=""><figcaption><p>Confirm</p></figcaption></figure>

### 步骤6：等待审核

模板由Meta审核，请耐心等待。一般情况下会在1天内完成审核。



审核失败：若模板被拒绝，可进入编辑页面查看原因，根据提示来修改模板或进行申诉。

<figure><img src="../../../.gitbook/assets/image (288).png" alt=""><figcaption><p>Rejected template</p></figcaption></figure>





## 验证码模板创建介绍

验证码模板的创建步骤同上，下文主要介绍验证码模板的设置项。

### Code delivery&#x20;

Code delivery是设置验证码送达的方式，方式有3种，分别为：

* [复制验证码](./#fu-zhi-yan-zheng-ma-de-mu-ban)
* [一键填充验证码](./#yi-jian-tian-chong-yan-zheng-ma)
* [零点击自动填充验证码](./#ling-dian-ji-yan-zheng-ma-mu-ban)

#### 复制验证码的模板

选择Copy Code类型的发送方式。可以自定义按钮的名称。[点击查看详细介绍](../../../whatsapp-ji-chu/xiao-xi-mu-ban/shen-fen-yan-zheng-xiao-xi-mu-ban/fu-zhi-yan-zheng-ma-shen-fen-yan-zheng-mu-ban.md)

<figure><img src="../../../.gitbook/assets/image (91).png" alt=""><figcaption></figcaption></figure>

#### 一键填充验证码

选择Autofill类型的发送方式。可以自定义按钮的名。Autofill 模式的验证码需要输入您的App的Package name，以及App signature hash。使用一键填充验证码要求您的应用必须能够启动“握手”[点击查看详细介绍](../../../whatsapp-ji-chu/xiao-xi-mu-ban/shen-fen-yan-zheng-xiao-xi-mu-ban/yi-jian-zi-dong-tian-chong-shen-fen-yan-zheng-mu-ban.md)

<figure><img src="../../../.gitbook/assets/image (90).png" alt=""><figcaption></figcaption></figure>

#### 零点击验证码模板

选择Autofill类型的发送方式。并填写完成Autofill的信息配置。开启Zero-tap按钮，并同意协议。

零点击验证码是一键填充验证码模板的升级，所以同样也要求您的应用必须能够启动“握手”[点击查看详细介绍](./#ling-dian-ji-yan-zheng-ma-mu-ban)

<figure><img src="../../../.gitbook/assets/image (92).png" alt=""><figcaption></figcaption></figure>

### 模板内容设置

虽然验证码模板内容是固定的，您仍然可以通过开关的方式增加验证码时效性提示和安全提示。

<figure><img src="../../../.gitbook/assets/image (93).png" alt=""><figcaption></figcaption></figure>



### 验证码消息有效时间配置

由于WhatsApp business api的消息是30天的有效性，也就是在发送后，30天内客户都可以打开WhatsApp查看消息，从而导致接收成功，消息接收成功后即收费。但是30天的有效性对于验证码消息来说太长了，大多数验证码都是在几分钟内才有效，所以在验证码模板上，WhatsApp提供了设置消息有效性的时间配置。

**功能：**&#x5728;此验证码模板消息发出后，在设置的消息有效时间内，若消息没有被成功接收，则不会继续尝试发送。即不会产生费用。**我们强烈建议您设置消息的有效时间小于或者等于您实际验证码的有效时间**。

举例：_您配置的消息有效时间是5分钟（实际验证码在您app里的有效时间可能是10分钟）。_

_WhatsApp下发了验证码消息给到用户，但由于用户未联网或其他原因，消息一直停留在processing（下发中）的状态，持续此状态5分钟后，WhatsApp会停止继续向此用户发送这条消息，这条消息就不会产生费用。即使用户在5分钟后连上网络打开WhatsApp也不会看到这条消息。_

配置入口 ：

<figure><img src="../../../.gitbook/assets/image (94).png" alt=""><figcaption></figcaption></figure>

## 相关阅读

{% content-ref url="../../../whatsapp-ji-chu/xiao-xi-mu-ban/" %}
[xiao-xi-mu-ban](../../../whatsapp-ji-chu/xiao-xi-mu-ban/)
{% endcontent-ref %}



