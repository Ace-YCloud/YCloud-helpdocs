---
doc_id: doc_whatsapp_accounts_zhang_hao_guan_li_chuang_jian_whatsapp_api_zhang_hao_whatsapp_business_app_coexistence
language: zh-CN
title: "WhatsApp Business App共存"
slug: whatsapp-business-app-coexistence
path: whatsapp-accounts-zhang-hao-guan-li/chuang-jian-whatsapp-api-zhang-hao/whatsapp-business-app-coexistence
document_group: whatsapp-accounts-zhang-hao-guan-li
path_in_group: chuang-jian-whatsapp-api-zhang-hao/whatsapp-business-app-coexistence
parent_id: doc_whatsapp_accounts_zhang_hao_guan_li_chuang_jian_whatsapp_api_zhang_hao
order: 0
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T07:24:27.456Z
updated_at: 2026-04-02T07:24:27.456Z
last_synced_at: 2026-04-02T07:24:27.456Z
tags:
---

# WhatsApp Business App共存

## 什么是 WhatsApp Coexistence

**这意味着您的WhatsApp Business API和WhatsApp Business App现在可以共存！**

这项功能支持将已经在WhatsApp Business App中使用的号码接入API，允许同一号码在API和App上同时运行。您可以在保留原本WhatsApp Business App使用习惯的同时，利用API提供的大规模群发消息、Chatbot智能AI 与工作流、Journey 客户运营等功能的优势，为您的业务带来巨大的增长。

此功能非常适合希望在继续使用WhatsApp Business App的同时扩展业务，逐渐过度到基于 API 的工作流程的团队。

## 使用WhatsApp Coexistence的好处

**场景1：**&#x5982;果您的员工需要在白天使用工作电脑与客户进行沟通，并在晚上通过App继续无缝服务客户。

**✅ 相应的好处：**&#x6D88;息将在App和 API 之间镜像传递。也就是说：

* 通过 API 发送的消息将显示在 WhatsApp Business App 中
* 通过WhatsApp Business App发送的消息将显示在Cloud API的对话历史记录中，可在PC端查看

**场景2：**&#x5982;果您想使用批量营销消息、智能Chatbot自动回复、基于Journey的客户运营等高级功能，同时保留App 上一对一对话的使用习惯。

**✅ 相应的好处：**&#x57;hatsApp Coexistence 支持您使用所有上述 API 功能的同时，为您保留WhatsApp Business App上发送一对一消息的功能。

**场景3：**&#x5982;果您已经有使用中的 WhatsApp Business App 号码，又想省去注册 API 账号的一系列繁琐步骤。

**✅ 相应的好处：**&#x652F;持无缝使用原WhatsApp Business App 号码接入 API 平台，您无需注销Business App 端的账号腾出号码来注册 API账号。

## 需要注意的信息

#### **限制**

1. 此功能**不支持以下这些国家的商家** （根据Business App电话号码确定）：尼日利亚、南非。
2. WhatsApp Business App账号每秒可发送消息上限为 5 条（包括手机端 app 发送的消息以及通过平台绑定后发出的消息，一起计算）

#### **App 版本要求**

要使用此功能，您必须使用WhatsApp Business App程序版本2.24.17或更高版本。

#### **定价**

从WhatsApp Business App发送的消息仍然是免费的,从API合作伙伴平台发送的消息将根据现有的[API定价模式](https://www.ycloud.com/price)收费。

#### **绑定后的功能对比**

以下表格描述了已加入Cloud API的企业客户可用的功能，以及在加入后WhatsApp Business应用功能的变化。注意：超过14天的媒体消息（如包含图片、视频、音频的消息）将无法进行同步。

<figure><img src="../../.gitbook/assets/image (964).png" alt=""><figcaption></figcaption></figure>

## 如何使用WhatsApp Business app 共存？

### 绑定 WhatsApp Business App

点击Create channels

<figure><img src="../../.gitbook/assets/My_Photor_1751251354905.jpg" alt=""><figcaption></figcaption></figure>

选择WhatsApp Business APP Coexistence

<figure><img src="../../.gitbook/assets/My_Photor_1751271717035.jpg" alt=""><figcaption></figcaption></figure>

然后在弹出窗口中选择使用 WhatsApp Business app 登录

<figure><img src="../../.gitbook/assets/My_Photor_1756783348516.jpg" alt="" width="351"><figcaption></figcaption></figure>

输入您需要绑定的WhatsApp Business app号码，点击下一步继续

<figure><img src="../../.gitbook/assets/My_Photor_1756784345898.jpg" alt="" width="351"><figcaption></figcaption></figure>

屏幕上将会出现一个二维码，使用您的手机WhatsApp Business app扫描该二维码进行绑定

<figure><img src="../../.gitbook/assets/My_Photor_1756784609459.jpg" alt="" width="351"><figcaption></figcaption></figure>

WhatsApp 消息将引导你使用该应用扫描嵌入式注册页面中显示的二维码。点击该按钮后，您可以选择同步近 6 个月的历史消息记录到平台

<figure><img src="../../.gitbook/assets/image (113).png" alt="" width="188"><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (115).png" alt="" width="188"><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (70).png" alt="" width="188"><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (71).png" alt="" width="188"><figcaption></figcaption></figure>

进入授权页面，点击继续按钮

<figure><img src="../../.gitbook/assets/My_Photor_1756784902943.jpg" alt="" width="331"><figcaption></figcaption></figure>

注意商业名称必须填注册文件上一模一样的名字，否则会影响未来的企业认证导致无法发送消息。

如果您的业务有官网，请正确复制粘贴网站信息，否则请勾选“我的业务没有网站”

<figure><img src="../../.gitbook/assets/image (27).png" alt="" width="375"><figcaption></figcaption></figure>

点击确认按钮完成授权绑定

<figure><img src="../../.gitbook/assets/My_Photor_1756785010152.jpg" alt="" width="331"><figcaption></figcaption></figure>

页面将显示正在绑定中，稍作等待

<figure><img src="../../.gitbook/assets/My_Photor_1756785089309.jpg" alt="" width="331"><figcaption></figcaption></figure>

完成绑定后将显示以下页面，点击结束按钮，系统将自动跳转，请等待系统跳转回到账号列表页

<figure><img src="../../.gitbook/assets/My_Photor_1756785117009.jpg" alt="" width="331"><figcaption></figcaption></figure>

在完成授权后，如果您授权同步您的聊天记录，我们将立即开始同步您的聊天内容。在同步过程中请保持WhatsApp Business应用程序打开，并注意在同步完成后新消息才会显示在Inbox中。

<figure><img src="../../.gitbook/assets/image (117).png" alt=""><figcaption></figcaption></figure>

您会看到一个特殊的图标，表示这个号码来自WhatsApp Business App。

<figure><img src="../../.gitbook/assets/image (119).png" alt=""><figcaption></figcaption></figure>

### 解绑 WhatsApp Business App

您必须通过手机上的 WhatsApp Business App 进行解绑操作，点击设置-账户-商业平台，然后点击您已经绑定的商业平台进行解绑。

**IOS**：

<figure><img src="../../.gitbook/assets/image (956).png" alt="" width="188"><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (957).png" alt="" width="188"><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (958).png" alt="" width="188"><figcaption></figcaption></figure>

**Android**:

<figure><img src="../../.gitbook/assets/image (959).png" alt="" width="188"><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (960).png" alt="" width="188"><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (961).png" alt="" width="188"><figcaption></figcaption></figure>



## 观看教程演示视频👇

{% embed url="https://www.bilibili.com/video/BV1fHa6zGEjK/" %}
