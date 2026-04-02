---
doc_id: doc_inbox_zui_jia_shi_jian_fu_wu_tuan_dui_ru_he_shi_yong_inbox
language: zh-CN
title: "服务团队如何使用Inbox"
slug: fu-wu-tuan-dui-ru-he-shi-yong-inbox
path: inbox/zui-jia-shi-jian/fu-wu-tuan-dui-ru-he-shi-yong-inbox
document_group: inbox
path_in_group: zui-jia-shi-jian/fu-wu-tuan-dui-ru-he-shi-yong-inbox
parent_id: doc_inbox_zui_jia_shi_jian
order: 20
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T11:14:41.208Z
updated_at: 2026-04-02T11:14:41.208Z
last_synced_at: 2026-04-02T11:14:41.208Z
tags:
---

# 服务团队如何使用Inbox

Inbox 作为 YCloud 中的一项重要功能，为服务团队提供了一个高效便捷的客户沟通与管理平台。为了帮助服务团队充分发挥 Inbox 的优势，以下是一系列最佳实践。

## 服务团队主管

### WABA账号的创建及客服的邀请

* 创建一个WABA账号，添加一个号码
* 邀请客服为Service角色
* 创建团队，例如“售前”、“售后”，将对应坐席添加到对应团队中

这样配置可将所有坐席与同一个号码管理，实现坐席分配的效果。

### 设置分配规则

<figure><img src="../../.gitbook/assets/image (540).png" alt=""><figcaption></figcaption></figure>

* 在号码中选中“依次将新会话自动分配给列表中的在线人员”，将“售前”团队加入列表中。
* 打开高级分配规则：开启将会话优先分配给上一次接待的坐席。

该设置可让会话自动依次分配给在线坐席，同时保证用户再次有问题时可联系到之前接待过的坐席

### 设置自动化（可选）

按照企业需求为号码配置自动化的欢迎消息及自动消息回复。

详情参考 [自动化](../../whatsapp-accounts-zhang-hao-guan-li/shou-ji-hao-ma-guan-li/zi-dong-hua.md)

### 设置标签

设置企业通用标签，帮助管理并分类客户。

1. 根据常见的客户需求和问题类型设置标签,如"新用户咨询"、"产品投诉"、"订单问题"、"技术支持"等。这样能快速区分和处理不同类型的客户需求。
2. 对于紧急或需要优先处理的情况,设置"高优先级"标签。这可以确保关键问题得到及时关注和解决。
3. 为不同的客户级别或VIP客户设置相应的标签,如"黄金客户"、"白金客户"等。这有助于给予重点客户更优质的服务。
4. 设置"待处理"、"已回复"、"已解决"等状态标签,跟踪服务的处理进度。

### 设置Contact属性

定义团队重点跟进记录的信息，添加为contact属性。例如：定义“备注”，字段为“文本”。客服可在聊天中可记录该项信息。更好的了解客户信息

<figure><img src="../../.gitbook/assets/image (535).png" alt=""><figcaption></figcaption></figure>

### 定义快捷回复

设置团队通用的[快捷回复](../kuai-jie-hui-fu.md)

左下角的头像Account进入 点击 [Edit](https://www.ycloud.com/console/#/app/userSettings/myProfile) > [Canned response](https://www.ycloud.com/console/#/app/userSettings/cannedResponse) > Add Canned Response

* 分析常见客户问题类型\
  仔细分析客户常见的咨询、投诉或疑问类型,如产品使用、订单状态、退换货等。这是制定快捷回复的基础。
* 梳理标准解决方案\
  针对每种常见问题,制定标准的解决方案和回复流程。可以包括问题描述、解决步骤、承诺时间等。
* 编写简洁高效的回复模板\
  根据标准解决方案,编写简明扼要的回复模板。注意语言简洁、措辞礼貌,避免冗长烦琐的表述。

例如：

1. 用户感谢\
   "您好,非常感谢您的询问。如有任何其他问题,欢迎随时告诉我。祝您购物愉快!"
2. 退换货\
   "亲爱的客户,我很抱歉您对商品不满意。根据我们的退换货政策,您可以在收到商品\[天数]内申请退换货。请您登录网站填写退货申请,我们会尽快为您处理。如有疑问随时告诉我。"
3. 产品咨询\
   "非常感谢您对我们产品的关注。\[产品名称]具有\[产品亮点]等特点,非常适合\[目标人群]使用。如您还有其他问题,欢迎随时咨询,我会耐心为您解答。"
4. 投诉处理\
   "您好,我理解您的不满情绪。作为客户的满意是我们的首要目标。请您告诉我具体的问题,我会尽快协调处理,并采取补救措施。给您带来不便,再次向您道歉,我们会努力提升服务质量。"
5. 技术支持\
   "很抱歉您在使用过程中遇到了问题。根据您描述的情况,我建议您尝试\[解决步骤]。如果问题仍未解决,请您提供\[所需信息],我会尽快为您查找原因并提供帮助。感谢您的耐心等待。"

### 查看Inbox分析

通过实时统计数据了解客服实时的接待情况



## 坐席

点击左侧导航栏Inbox，作为管理员/客服，你可以在这里查看到WhatsApp所有的消息。

#### 个人状态设置

登陆后，状态是“Away”，请将个人状态调整状态为“Available”，新接入的会话才能被自动分配给你。

<figure><img src="../../.gitbook/assets/image (539).png" alt=""><figcaption></figcaption></figure>

### 用好客户详情

给客户打标签可以更好的对客户分类管理、优先处理重点客户、提高客户体验。

<figure><img src="../../.gitbook/assets/image (552).png" alt=""><figcaption></figcaption></figure>

### 转接会话

当遇到无法处理的客户问题，将会话转交给专业团队或坐席。

<figure><img src="../../.gitbook/assets/image (551).png" alt=""><figcaption></figcaption></figure>

