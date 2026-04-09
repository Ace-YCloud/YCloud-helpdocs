---
description: 本文介绍如何使用 YCloud 配置 Meta （包含Instagram/Facebook） 到 WhatsApp 的消息广告链路。
---

# Meta CTWA 广告

完成本组配置后，您可以在 Facebook 或 Instagram 投放跳转到 WhatsApp 的广告，将潜在客户直接引导到 WhatsApp 对话，并通过 YCloud 统一承接线索、回传转化事件和查看广告数据。本文用于帮助您了解 Meta CTWA 的前置准备、关键配置点和完整操作流程。

{% hint style="info" %}
如果您还不了解 CTWA 的基本概念，建议先阅读：

* [CTWA介绍](https://helpdocs.ycloud.com/help-center/zh/ctwa-click-to-whatsapp-ad/ctwa-jie-shao)
{% endhint %}

### 什么是 Meta CTWA 广告

Meta CTWA 广告是指用户在 Facebook 或 Instagram 看到广告后，点击广告中的按钮，直接进入 WhatsApp 与企业开始对话的广告形式。

对于企业来说，这类广告的重点不只是获得一次点击，而是让用户更快进入会话，并在 YCloud 中完成后续承接、跟进和转化优化。

### 实际投放效果示意

下图展示了用户在 Facebook 或 Instagram 中看到广告、点击 CTA 后跳转到 WhatsApp 发起会话的效果。

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2FHcSx0cvAUeGjZ68PMLnX%2Ffacebook-wa%20(1).gif?alt=media&#x26;token=83aa7ae7-0b2c-42a2-8149-2f32c08c3638" alt=""><figcaption></figcaption></figure>



### Meta 方案的关键配置点

在 Meta CTWA 场景中，广告账户、Facebook Page、Instagram 账号和 WhatsApp Business 号码之间的关系，会直接影响广告能否顺利创建和投放。

开始前，建议先确认这些核心资产已经准备完成：

* 可正常使用的 Meta 广告账户
* 已接入 YCloud 的 WhatsApp Business 号码
* 用于投放的 Facebook Page
* 当前操作人拥有对应资产的管理权限

### Meta 投放前需要确认的账号关系

在 Meta CTWA 场景中，不同投放位置对应的资产准备略有区别。建议您先确认以下关系是否已配置完成。

<table><thead><tr><th width="111.51171875">投放位置</th><th>需要确认的关系</th><th>说明</th></tr></thead><tbody><tr><td>Facebook</td><td>Facebook Page 已关联用于承接会话的 WhatsApp Business 号码✅</td><td>创建点击 WhatsApp 广告时，您需要基于对应的 Facebook Page 完成广告配置</td></tr><tr><td>Instagram</td><td><p>Instagram 专业账号已连接到对应的 Facebook Page✅</p><p><strong>且</strong></p><p>该 Facebook Page 已关联用于承接会话的 WhatsApp Business 号码✅</p></td><td>如果广告投放到 Instagram，除了 WhatsApp 关联外，还需要确保 Instagram 账号与 Facebook Page 的关系已配置完成</td></tr></tbody></table>

### 开始前准备

在进入正式配置前，建议先确认以下内容已经准备完成。

#### Meta 侧准备

* 可正常使用的 Meta 广告账户
* 对目标 Business Manager、广告账户和 Facebook Page 的管理权限
* 用于投放的 Facebook Page
* 如果计划在 Instagram 投放，请确认对应的 Instagram 专业账号已准备完成并可正常使用

#### YCloud 侧准备

* 可正常登录的 YCloud 账号
* 已接入 YCloud 的 WhatsApp Business 号码
* 能够及时处理 WhatsApp 咨询的销售或客服团队

如果您还没有在 YCloud 中接入 WhatsApp Business 号码，请先完成号码接入：

* [添加 WhatsApp Business 号码](https://helpdocs.ycloud.com/help-center/zh/whatsapp-accounts-zhang-hao-guan-li/chuang-jian-whatsapp-api-zhang-hao/tong-guo-qian-ru-shi-zhu-ce-chuang-jian-waba)

### 配置流程总览

Meta CTWA 广告的完整流程分为以下 3 个环节：

1. 在 YCloud 中连接 Meta 广告账户
2. 在 Meta Ads Manager 中创建点击 WhatsApp 广告
3. 配置转化回传，并在 Meta 与 YCloud 中查看广告与转化数据

下图展示了 YCloud 与 Meta Ads Manager 之间的主要配置流程：

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2FnamBhmaIM87NyCdXb7pX%2Fflow-ycloud%26meta%20ad%20manager.png?alt=media&#x26;token=2b03f3ef-7719-4e2d-bc8b-57b69647bfb5" alt=""><figcaption></figcaption></figure>

### 操作步骤

#### 第一步：连接 Meta 广告账户

在 YCloud 中完成 Meta 广告账户授权后，YCloud 才能读取广告相关信息，并支持后续的转化回传和数据查看。

* [连接Meta广告帐户](https://helpdocs.ycloud.com/help-center/zh/ctwa-click-to-whatsapp-ad/facebook-ads/connect-facebook-ad-account)

#### 第二步：创建点击 WhatsApp 广告

在 Ads Manager 中，您需要完成广告目标选择、Page 与 WhatsApp 关联、广告组设置、广告创意配置等步骤。

* [创建点击WhatsApp广告（CTWA）](https://helpdocs.ycloud.com/help-center/zh/ctwa-click-to-whatsapp-ad/facebook-ads/chuang-jian-dian-ji-whatsapp-guang-gao-ctwa)

#### 第三步：配置转化回传与查看数据

广告上线后，您可以继续在 YCloud 中配置转化回传规则，并分别在 Meta 与 YCloud 中查看会话、转化和数据表现。

* [Meta广告：流量承接、转化回传](https://helpdocs.ycloud.com/help-center/zh/ctwa-click-to-whatsapp-ad/facebook-ads/zhuan-hua-api-capi)

### 进一步使用

如果您已经开始投放广告，也可以继续查看以下相关文档：

* [接待CTWA的访客](https://helpdocs.ycloud.com/help-center/zh/ctwa-click-to-whatsapp-ad/jie-dai-ctwa-de-fang-ke)
* [CTWA分析](https://helpdocs.ycloud.com/help-center/zh/ctwa-click-to-whatsapp-ad/ctwa-fen-xi)
