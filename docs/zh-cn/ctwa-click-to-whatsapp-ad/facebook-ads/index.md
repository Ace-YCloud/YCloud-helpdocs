---
doc_id: doc_ctwa_click_to_whatsapp_ad_facebook_ads
language: zh-CN
title: "Meta CTWA 广告"
slug: facebook-ads
path: ctwa-click-to-whatsapp-ad/facebook-ads
document_group: ctwa-click-to-whatsapp-ad
path_in_group: facebook-ads
parent_id: doc_ctwa_click_to_whatsapp_ad
order: 710
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T11:13:30.710Z
updated_at: 2026-04-02T11:13:30.710Z
last_synced_at: 2026-04-02T11:13:30.710Z
tags:
---

# Meta CTWA 广告

#### 概述 <a href="#gai-shu" id="gai-shu"></a>

按本篇指引完成配置后，您可以实现： 在 Instagram/Facebook 投放跳转到 WhatsApp 的消息广告，将广告流量直接引导至 WhatsApp 对话，并通过 YCloud Inbox 统一承接和跟进潜在客户会话。

下文将依次介绍：前期准备、广告账户授权、创建CTWA广告，以及追踪与转化设置。

#### 什么是 Meta CTWA 广告？ <a href="#shen-me-shi-tiktok-xiao-xi-guang-gao" id="shen-me-shi-tiktok-xiao-xi-guang-gao"></a>

Meta CTWA 消息广告是一种帮助企业通过广告与潜在客户发起对话的广告形式。

{% hint style="info" %}
一句话介绍：用户在Fcebook、Instagram 浏览广告并点击后，跳转到WhatsApp 与您的Whsatsapp商业号码 沟通。
{% endhint %}

#### 为什么选择 Meta CTWA  广告？ <a href="#wei-shen-me-xuan-ze-tiktok-xiao-xi-guang-gao" id="wei-shen-me-xuan-ze-tiktok-xiao-xi-guang-gao"></a>

对于以咨询、留资和销售转化为目标的业务来说，Meta CTWA广告可以提供更直接的客户沟通路径。与“广告点击后进入落地页，再提交表单”的方式相比，这种广告形式更适合需要快速响应客户咨询的场景，主要体现在以下几个方面：

* 将广告流量直接引导至 WhatsApp，对话路径更短。
* 用户发起咨询后，可由 YCloud Inbox 统一承接和跟进。
* 结合会话事件和转化回传，有助于持续优化广告投放效果。

#### 实际投放效果示意 <a href="#shi-ji-tou-fang-xiao-guo-shi-yi" id="shi-ji-tou-fang-xiao-guo-shi-yi"></a>

下图演示：

用户在 Instagram\Facebook 中看到广告，在点击 CTA 后跳转到 WhatsApp 发起会话的实际效果。

<figure><img src="../../.gitbook/assets/facebook-wa (1).gif" alt=""><figcaption></figcaption></figure>

### 客户准备工作 <a href="#ke-hu-qian-qi-zhun-bei-gong-zuo" id="ke-hu-qian-qi-zhun-bei-gong-zuo"></a>

开始配置前，请按👇流程和清单，做好准备。



#### 准备清单

**Meta 侧准备**

* [了解Meta的概念：账号、资产](/broken/pages/LcYcMDje6hcgXDmmL7cW)
* Meta广告账号。点此[前往Meta广告管理平台 ](https://www.facebook.com/business/tools/ads-manager)
* 准备 **Facebook Page** 或 **Instagram 账号**（看广告投到哪里），用于绑定 WhatsApp 号码并承接广告。参考：[连接 Facebook Page 和 WhatsApp](https://www.facebook.com/help/2783732558314697/)



**YCloud 侧准备**

* 注册YCloud。[点此注册YCloud](https://www.ycloud.com/console/#/entry/register?)
* 在 YCloud 创建 WABA。点此了解：[创建 WhatsApp Business API 账户](https://helpdocs.ycloud.com/help-center/quick-start/create-a-whatsapp-business-api-account)、[通过 Embedded Sign-up 创建 WABA](https://helpdocs.ycloud.com/help-center/whatsapp-accounts-management/create-a-whatsapp-api-account/create-waba-via-embedded-sign-up)。
* 绑定投放的 WhatsApp Business 号码已在YCloud后台。如下图：

![](https://helpdocs.ycloud.com/help-center/~gitbook/image?url=https%3A%2F%2F4253554051-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F78HV6e8vN6mhwsbohgTK%252Fuploads%252FgT4Z0lnoYDLCQnExjAno%252FWHATSAPP_ACCOUNT-CONNECTED.png%3Falt%3Dmedia%26token%3D78df2040-fa16-40e7-91e1-196ab3636fd9\&width=768\&dpr=3\&quality=100\&sign=1cdc405b\&sv=2)

* 如果您尚未绑定，请先点此：[添加WhatsApp 商业号码](https://helpdocs.ycloud.com/help-center/zh/whatsapp-accounts-zhang-hao-guan-li/chuang-jian-whatsapp-api-zhang-hao/tong-guo-qian-ru-shi-zhu-ce-chuang-jian-waba)。

#### **实际操作流程**

<figure><img src="../../.gitbook/assets/flow-ycloud&#x26;meta ad manager.png" alt=""><figcaption></figcaption></figure>



#### 操作步骤 <a href="#cao-zuo-bu-zhou" id="cao-zuo-bu-zhou"></a>

1. 步骤1：[授权Meta广告账号到YCloud](connect-facebook-ad-account.md)
2. 步骤2：[创建Meta 点击WhatsApp广告（CTWA）](chuang-jian-dian-ji-whatsapp-guang-gao-ctwa.md)
3. 步骤3：[Meta广告：CAPI转化事件的设置与上报。](zhuan-hua-api-capi.md)
4. 步骤4：[在YCloud与广告流量对话](../jie-dai-ctwa-de-fang-ke.md)
