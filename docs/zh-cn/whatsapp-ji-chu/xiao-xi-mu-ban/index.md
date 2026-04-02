---
doc_id: doc_whatsapp_ji_chu_xiao_xi_mu_ban
language: zh-CN
title: "消息模板"
slug: xiao-xi-mu-ban
path: whatsapp-ji-chu/xiao-xi-mu-ban
document_group: whatsapp-ji-chu
path_in_group: xiao-xi-mu-ban
parent_id: doc_whatsapp_ji_chu
order: 130
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

# 消息模板

模板消息用于与客户开启营销、通知和身份验证[对话](https://developers.facebook.com/docs/whatsapp/pricing#conversations)。与自由格式消息不同，模板消息是唯一可以发送给尚未向您发送消息或过去 24 小时内未向您发送消息的客户的消息类型。

模板必须预先获得批准，然后才能被发送。此外，模板可能会根据客户反馈和参与度自动禁用。禁用后，模板将无法发送，直到其质量评级提高。

## 消息模板的类别

不同的消息模板对应不同的对话计费，请参考

* 身份验证：使用此类别发送验证码。
* 通知类型：使用此类别发送帐户更新、订单更新、警报和其他重要信息
* 营销类型：使用此类别发送促销优惠、产品公告和其他与营销相关的信息，以提高知名度和参与度。

## 消息模板的内容

消息模板包括以下内容：

* 标题：此部分可以包含徽标或其他品牌元素，以及标题或视频。
* 正文：正文是邮件的主要内容。它应包含所有相关信息，并以清晰简洁的方式编写。
* 页脚：页脚可以包含其他消息，例如号召性用语或联系信息。
* 按钮：按钮是可选元素，可包含在您的消息中，以鼓励收件人采取特定的操作，例如访问网站或进行购买。

<figure><img src="../../.gitbook/assets/image (512).png" alt=""><figcaption></figcaption></figure>

## 创建模板

使用API创建模板，请参考

{% embed url="https://docs.ycloud.com/reference/whatsapp-template-creation-examples" %}

使用YCloud管理后台创建模板，请参考：

{% content-ref url="../../whatsapp-accounts-zhang-hao-guan-li/mu-ban-guan-li/chuang-jian-mu-ban/" %}
[chuang-jian-mu-ban](../../whatsapp-accounts-zhang-hao-guan-li/mu-ban-guan-li/chuang-jian-mu-ban/)
{% endcontent-ref %}



## 模板审核

创建模板后，您可以提交模板以供审批。审批决定最多可能需要 24 小时。一旦做出决定，您的 BM帐户 管理员会收到电子邮件。

如果您的消息模板获得批准，其状态将设置&#x4E3A;**“有效 - 质量待定”**，您可以开始将其发送给客户。如果被拒绝，您可以编辑并重新提交以供批准，或对决定[提出上诉。](https://developers.facebook.com/docs/whatsapp/message-templates/guidelines#appeals)



## 常见的拒绝原因

提交通常由于以下原因被拒绝，因此请确保避免这些错误。

* 变量参数缺失或花括号不匹配。正确的格式是`{{1}}`。
* 变量参数包含特殊字符，例如`#`、`$`或`%`。
* 变量参数不具有连续性。例如，`{{1}}`，`{{2}}`，`{{4}}`，`{{5}}`已定义但`{{3}}`不存在。
* 消息模板包含违反 WhatsApp 商业政策的内容：当您提供商品或服务进行销售时，我们会将与您的商品或服务相关的所有消息和媒体（包括任何描述、价格、费用、税费和/或任何所需的法律披露）视为构成交易。交易必须遵守[WhatsApp 商业政策](https://l.facebook.com/l.php?u=https%3A%2F%2Fwww.whatsapp.com%2Flegal%2Fcommerce-policy%2F%3Ffbclid%3DIwZXh0bgNhZW0CMTEAAR0iHyU-k_AwIfmWxcKhpU0r6N7j7cUQ5DiZhdWTwwcdGCYRbL8RlpXxjmU_aem_7IzIW0N0jczoJq2N1oCR9g\&h=AT0gd0XysVbil3TL2mhX2kxvQfmDSn03g8volglJ6oaup-VJHWL0H1Fys3-vo5lMsHAsiQStQyjUV_9szwUgdKdXe5vm__e17KfP7tK6kgx-YeTwRQ-eRs5N6SbAXwKKVIrVD4TNTkU)。
* 消息模板包含违反[WhatsApp 商业政策的](https://www.whatsapp.com/legal/business-policy/?fbclid=IwZXh0bgNhZW0CMTEAAR18bv6_VUkTHb-vQvPBuoA2l_Pu2NCWOGTvRVOoznQEJpYA8AE1Nsu3NNw_aem_q2mmaMbLCKvp4KQDCgwDrw)内容：不要向用户索要敏感标识符。例如，不要要求人们分享完整的个人支付卡号、金融账户号、国民身份证号码或其他敏感标识符。这还包括不向用户索要可能包含敏感标识符的文件。请求部分标识符（例如：社会安全号码的最后 4 位数字）是可以的。
* 该内容包含潜在的辱骂或威胁内容，例如威胁对客户采取法律行动或威胁公开羞辱他们。
* 该消息模板与现有模板重复。如果提交的模板正文和页脚中的措辞与现有模板相同，则重复的模板将被拒绝。

拒绝信息也将通过电子邮件发送给BM的管理员

如果您认为模板被拒绝是不正确的，您可以提交[模板申诉](./#mu-ban-shen-su)。也可以选择编辑被拒绝模板并重新提交。

此检查不适用于归类为 的模板`AUTHENTICATION`。



## 模板状态

以下是 WhatsApp 模板可以具有的状态：

* 审核中：表示模板仍在审核中。审核最多可能需要 24 小时。
* 已拒绝：该模板在我们的审核过程中被拒绝或违反了我们的一项或多项政策。
* 活跃 - 质量待定：消息模板尚未收到客户的质量反馈。此状态的消息模板可以发送给客户。
* 活跃 - 高质量：模板几乎没有收到任何负面客户反馈。具有此状态的消息模板可以发送给客户。
* 活跃 - 中等质量：该模板已收到多位客户的负面反馈，但可能很快会被暂停或禁用。此状态的消息模板可以发送给客户。
* 活跃 - 质量低下：该模板已收到多位客户的负面反馈。此状态的消息模板可以发送给客户，但很快面临被暂停或禁用的风险。
* 已暂停：由于客户反复给出负面反馈，该模板已暂停。处于此状态的消息模板无法发送给客户。
* 已禁用：由于客户反复给出负面反馈，该模板已被禁用。处于此状态的消息模板无法发送给客户。
* 已上诉 - 审查中：表示已请求上诉。



## 模板暂停

如果最终用户反复举报垃圾邮件或屏蔽与某个消息模板相关的消息，WhatsApp 会暂停该模板一段时间，以保护使用该模板的发件人的质量评级。暂停时长如下：

* 第一份报告：暂停 3 小时
* 第二次报告：暂停 6 小时
* 第三次报告：禁用

在模板暂停的几个小时内，您可以选择以下操作之一：

* 编辑模板内容：如果您认为模板内容可能会被最终用户视为垃圾邮件或网络钓鱼，请编辑内容。例如，删除模板中的特定词语。
* 重塑目标受众：如果您认为消息与当前目标受众不相关，请更改受众。例如，如果模板内容仅与特定忠诚度群体相关，则仅将模板消息发送给该群体，而不是发送给所有最终用户。\
  进行更改后，更新后的模板将在两分钟内生效。您无需等待三小时期限结束后再使用模板。Meta 将继续跟踪更新后的模板的最终用户阻止率。
* 不采取任何措施：三小时后模板将再次上线。但是，模板可能会再次被暂停。如果在暂停后继续使用低质量的模板，发件人质量以及最终的消息发送限制可能会受到影响。\
  <br>

## 模板申诉

如果您的提交被拒绝，您可以提出申诉。请注意，申诉必须包含示例。

你需要前往 登陆BM账户 > [Account Quality](https://business.facebook.com/business-support-home/), 对"Rejected template"提出申诉

1. &#x5728;**“**[**Account Quality**](https://business.facebook.com/business-support-home/)**”**&#x9875;面上，单&#x51FB;**“Rejected Template”**。
2. 从被拒绝的模板列表中选择，然后单&#x51FB;**“Request for Review”**。
3. 输入**申诉原因**并点&#x51FB;**"Submit"**。
4. 提交后，请求和问题将移&#x81F3;**“In Review”**&#x9009;项中。
5. 申诉审核决定将通过业务经理发送，通常需要 24 到 48 小时。申诉的违规行为将保&#x6301;**“Unchanged”（不变）**&#x6216;被设置&#x4E3A;**“Reversed”（撤销）**。

<figure><img src="../../.gitbook/assets/image (513).png" alt=""><figcaption></figcaption></figure>
