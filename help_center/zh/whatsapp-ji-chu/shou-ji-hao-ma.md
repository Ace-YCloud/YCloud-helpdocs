---
description: 本指南介绍如何选择电话号码、将其添加到您的WABA帐户以及相关的发送限制。
---

# 手机号码

WhatsApp 商业帐户 (WABA) 需要一个有效的电话号码才可以与客户进行消息互动。

## 向 WABA 添加电话号码

如果您现在还没有WABA，请通过嵌入式注册创建第一个WABA并连接手机号码。

{% content-ref url="../whatsapp-accounts-zhang-hao-guan-li/chuang-jian-whatsapp-api-zhang-hao/tong-guo-qian-ru-shi-zhu-ce-chuang-jian-waba.md" %}
[tong-guo-qian-ru-shi-zhu-ce-chuang-jian-waba.md](../whatsapp-accounts-zhang-hao-guan-li/chuang-jian-whatsapp-api-zhang-hao/tong-guo-qian-ru-shi-zhu-ce-chuang-jian-waba.md)
{% endcontent-ref %}

如果您已经拥有WABA，可以直接在YCloud后台 > WhatsApp Account 添加手机号码。

{% content-ref url="../whatsapp-accounts-zhang-hao-guan-li/chuang-jian-whatsapp-api-zhang-hao/tian-jia-hao-ma.md" %}
[tian-jia-hao-ma.md](../whatsapp-accounts-zhang-hao-guan-li/chuang-jian-whatsapp-api-zhang-hao/tian-jia-hao-ma.md)
{% endcontent-ref %}

## 迁移电话号码

如果您想使用已在 WhatsApp 或 WhatsApp Business 平台上注册的电话号码，请参阅我们的迁移指南

* [将现有的 WhatsApp 号码迁移至企业帐户](https://developers.facebook.com/docs/whatsapp/on-premises/get-started/migrate-existing-whatsapp-number-to-a-business-account)
* [将电话号码迁移至其他 WABA](../whatsapp-accounts-zhang-hao-guan-li/chuang-jian-whatsapp-api-zhang-hao/hao-ma-qian-yi.md)

## 电话号码注册数量限制

最初仅限注册 2 个商业电话号码。

如果您的企业已经过企业认证，最多将增加到20个。

如果您确实有足够的必要将限制增加到 20 以上，可以联系YCloud支持团队。

## 显示名称

每个电话号码都有显示名称，此名称应与您的公司名称或品牌名称相关。显示名称将由 Meta 审核。显示名称需要遵循 [显示名称指南](https://www.facebook.com/business/help/757569725593362)。

在YCloud里，您可以通过以下路径更改显示名称：YCloud > WhatsApp accounts > Number settings > Business Profile > Display name > Edit.&#x20;

<figure><img src="../.gitbook/assets/image (838).png" alt="111"><figcaption><p>在YCloud更改显示名称</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (841).png" alt=""><figcaption><p>点击Edit弹出弹窗</p></figcaption></figure>

⚠️注意：

* 建议您更改显示名称之前认真阅读WhatsApp Business display name guidelines.
* 显示名称限制在3-150个字符。

💡修改后显示名称将会呈现以下几种状态：

* Approved：代表您的显示名称已通过审核；
* Rejected：代表您的显示名称被拒绝；
* In review：代表您的显示名称正在审核中。



## 电话号码状态

状态分类如下：

* 已连接：发送功能正常。
* 已标记：当电话号码质量评级达到低（红色）状态时，将出现此状态。在此状态下，您无法升级消息限制层级。如果质量评级在已标记之日起 7 天内提高到中等或高状态，则状态将更改为已连接。如果质量评级没有提高，电话号码状态将恢复为已连接，但消息限制将降低到下一个较低的层级。
* 受限：当电话号码达到消息限制时，将出现此状态。在受限阶段，您无法主动与客户发送消息，直到 24 小时窗口重置为止。但您仍可以回复用户发起的消息。

## 质量评级

你的电话号码质量评级基于您聊天的人对您的消息的接受程度。它由商家和用户之间的对话中的多种质量信号决定。主要包括用户反馈信号（如屏蔽、举报）以及用户屏蔽商家时提供的原因。

因此，如果您发送的消息不受人们喜欢，他们屏蔽或举报您，您的评分就会下降。当你改善了发送内容或客户群体，您的评分就会回升。

要保持高评分，请确保您的消息有用且不会令人厌烦。

质量评级分为：

* 高：电话号码几乎没有收到负面客户反馈。
* 中：电话号码已收到一些客户的负面反馈。
* 低：电话号码收到多位客户的负面反馈。

请注意，流量大的号码在短时间内（甚至几分钟内）出现质量变化是正常的。

您可以在YCloud > WhatsApp accounts，查看电话号码质量：

<figure><img src="../.gitbook/assets/image (507).png" alt=""><figcaption><p>电话号码质量</p></figcaption></figure>

#### **保持高质量评级的一些建议** <a href="#maintain-high-quality-rating" id="maintain-high-quality-rating"></a>

为了保证您的信息传递的良好健康：

1. Meta 要求企业在开始对话之前获得客户的选择，无论是在 WhatsApp 上还是在 WhatsApp 之外都可以。
2. 确保消息符合 WhatsApp 商业政策和商务政策。
3. 为用户制作高度个性化和有益的信息，避免通用和开放式的介绍。
4. 谨慎控制消息频率，避免过多的日常交流，并优化信息消息的内容和长度。
5. 清楚地传达在 WhatsApp 上接收重要更新的价值，并保持消息的个性化。
6. 允许客户选择接收的消息类型并相应地尊重他们的选择。
7. 提供选择退出的方法，包含“**停止**”&#x6216;**“取消订阅**”按钮等功能。
8. 尊重客户请求，避免向退订用户发送消息，从而降低客户屏蔽或举报您的账号的风险。



## 消息限额

消息限制决定了您在连续 24 小时内可使用该电话号码发起的最大对话数量。这些限制不适用于用户发起的对话。

您可以在YCloud > WhatsApp accounts，查看电话号码消息限制：

<figure><img src="../.gitbook/assets/image (508).png" alt=""><figcaption><p>电话号码消息限制</p></figcaption></figure>



### 初始限额

未经过企业认证或未获批准显示名称的企业电话号码限制为250个/天。也就是说在24 小时内最多可以由企业发起 250 个对话。

经过企业认证且显示名称已获批准的电话号码，消息限制将提升为1000个/天。

在达到 1000个/天 消息限制之前，[**WhatsApp 管理器**](https://business.facebook.com/wa/manage/home/)>**概览**>**限制**面板会显示有关如何增加限制的有用信息。

<figure><img src="../.gitbook/assets/image (510).png" alt="" width="319"><figcaption></figcaption></figure>

### 提升限额

消息限制可以增加到以下水平：

* 1K 个由企业发起的对话
* 10K 个由企业发起的对话
* 10 万次由企业发起的对话
* 无限数量的业务发起对话

此数量从 1K 个唯一客户开始，并根据电话号码状态、电话号码质量评级以及企业与唯一客户发起对话的频率自动扩展。

#### 自动扩展规则

每次您与一位特定客户发起新对话时，WhatsApp 都会确定是否应增加您的限制。此决定基于以下标准：

* 您的电话号码状态为已连接
* 您的电话号码质量评级为“中”或“高”
* 在过去 7 天内，您与唯一客户发起了 X 次或更多次对话，其中 X 是您当前的消息传递限制除以 2\
  如果您满足所有条件，我们将在 24 小时内将您的消息传递限制提高一个级别。

你也可以在前往 [**WhatsApp 管理器**](https://business.facebook.com/wa/manage/home/)>**帐户工具**> **Insights，**&#x4E86;解您的企业电话号码将如何提升到下一个水平：

<figure><img src="../.gitbook/assets/image (511).png" alt=""><figcaption></figcaption></figure>



## 从 WABA 中删除电话号码

前往 BM帐户 > WhatsApp Manage > [Phone number](https://business.facebook.com/wa/manage/phone-numbers)

找到您想要删除的电话号码。点击垃圾桶图标。

<figure><img src="../.gitbook/assets/image (506).png" alt=""><figcaption><p>删除电话号码</p></figcaption></figure>

{% hint style="warning" %}
删除注意：

* 只有BM帐户管理员可以删除电话号码。
* 如果企业在过去 30 天内使用该号码发送过付费消息，则无法删除该号码。
* 从 WhatsApp 商业平台删除号码后，该号码可在 WhatsApp 应用程序中再次使用，或可在 WhatsApp 商业平台中再次注册。但对于已被 WhatsApp 商业平台禁止的手机号码不适用该规则。
{% endhint %}



<br>
