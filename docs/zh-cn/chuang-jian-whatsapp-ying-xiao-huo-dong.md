---
doc_id: doc_chuang_jian_whatsapp_ying_xiao_huo_dong
language: zh-CN
title: "创建WhatsApp营销活动"
slug: chuang-jian-whatsapp-ying-xiao-huo-dong
path: chuang-jian-whatsapp-ying-xiao-huo-dong
document_group: 
path_in_group: chuang-jian-whatsapp-ying-xiao-huo-dong
parent_id: 
order: 0
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T07:14:57.554Z
updated_at: 2026-04-02T07:14:57.554Z
last_synced_at: 2026-04-02T07:14:57.554Z
tags:
---

# 创建WhatsApp营销活动

{% hint style="info" %}
**什么是营销类型的会话/消息** 在WhatsApp中，您只需要拥有用户手机号（并征得用户同意），即可向他们发送消息。并且可以添加可点击的CTA 和快速回复按钮，使您的营销信息更具可操作性，以促进您的业务转化。 虽然WhatsApp API 看起来非常适合营销用途，但它设计的初衷绝对不仅是盲发拉新营销。假如你盲目地向潜在用户发送广告消息，很快会面临封号的处理。 实际上，在WhatsApp生态里还有很多可以挖掘的场景和用途，这方面可以充分参考国内微信公众号的成功经验，WhatsApp里也有丰富的工具性功能，用好了绝对事半功倍。
{% endhint %}

## 步骤1：创建营销模板

* 登录[YCloud账号](https://www.ycloud.com/console/#/entry/login)，导航至Home > Templates > Add Template

<figure><img src="../.gitbook/assets/image (542).png" alt=""><figcaption></figcaption></figure>

* Category选择Marketing，并命名模版名称和选择模版语言

请注意：**模版名称必须要唯一的**。名称仅支持小写字母a-z、0-9、 下划线（\_)。模版一旦提交，无法进行更改 &#x20;

<figure><img src="../.gitbook/assets/image (544).png" alt=""><figcaption></figcaption></figure>

* 输入要发送的内容\
  营销类消息用于发送促销优惠、产品公告和其他营销相关消息，以提高认知度和参与度。包括但不仅限于：
  * 促销或优惠消息
  * 欢迎语/结束语：i.e.: Thank you for shopping at XXX, wish you have a good day&#x20;
  * 更新，邀请，建议：i.e: Hey members, join us tonight for this event

<figure><img src="../.gitbook/assets/image (547).png" alt=""><figcaption></figcaption></figure>

* 点击Submit，并等待审核通过

<figure><img src="../.gitbook/assets/image (548).png" alt=""><figcaption></figcaption></figure>



## 步骤2：发送营销消息

{% hint style="info" %}
发送营销消息的方式有两种：Campaign发送或调用接口发送；您可任选其一
{% endhint %}

### 使用Campaign发送

#### 1. 选择用WhatsApp渠道发送群发消息

登录[YCloud账号](https://www.ycloud.com/console/#/entry/login), 导航至Campaign > + Add Campaign > WhatsApp

<figure><img src="../.gitbook/assets/image (549).png" alt=""><figcaption></figcaption></figure>

#### 2. 填写Campaign相关信息

2.1 给Campaign命名：也可选择默认命名

2.2 选择Sender：通过嵌入式流程绑定的api号码

2.3 选择通过meta审核的模板以及语言

2.4 发送时间：立即发送或预约发送时间

<figure><img src="../.gitbook/assets/image (550).png" alt=""><figcaption></figcaption></figure>

2.5 点击 Next，配置收件人

#### 3.选择收件人

{% hint style="info" %}
YCloud为您提供了多种方式，选择campaign活动的收件人：

1. 手动输入
2. 上传csv文件
3. 根据条件，筛选联系人
{% endhint %}



**3.1 手动输入**

{% hint style="info" %}
**请注意，**&#x5982;果模板中有变量，我们建议使用上传文件来设置收件人。手动输入仅支持将这些变量设置为固定值。\
&#xNAN;_&#x4F8B;如，模板是“Hi，\{{name\}} ”，而您选择使用手动输入来上传收件人，那么您只能将\{{name\}}设置为固定值，例如“there”。发送给所有收件人的最终消息将是“Hi, there”。_
{% endhint %}

在框中输入电话号码，每行只能输入一个号码。并且请确保号码为国际格式，以国家代码开头。例如，英国号码是44，电话号码是7759398257，则应输入+447759398257。 如果您已经有excel文件，则可以复制电话号码栏并粘贴到框中。

<figure><img src="../.gitbook/assets/image (643).png" alt=""><figcaption></figcaption></figure>

**3.2 上传csv文件**

上传文件方法支持在消息上**设置变量。**

* 下载模板，填写电话号码。

<figure><img src="../.gitbook/assets/My_Photor_1719294327955.jpg" alt=""><figcaption></figcaption></figure>

*   打开模板文件，填写电话号码

    * 电话号码必须在第一栏，并命名为“phone”。
    * 如果消息中没有任何变量，则可以删除模板的其他列。
    * 如果消息中有变量，则可以从第二列第一行开始输入变量名称

    _例如，短信是 “嗨，\{{name\}}熊猫袜子到了！有几种颜色”。然后你可以设置一个名为“ name ”的变量_

<figure><img src="../.gitbook/assets/image (646).png" alt=""><figcaption></figcaption></figure>

**3.3 筛选联系人**

{% hint style="info" %}
筛选，指：从您的联系人中，根据某些条件，筛选收件人。

YCloud提供 2种筛选方式

1. 选择：联系人分组
2. 选择：联系人特征
{% endhint %}

<figure><img src="../.gitbook/assets/campaign_20251009_step2_contactFilter.png" alt=""><figcaption></figcaption></figure>

3.3.1 选择：联系人分组

单击Contact Segment，

选择1个或多个分组。

<figure><img src="../.gitbook/assets/campaign_step2_contactFilter_segment.png" alt=""><figcaption></figcaption></figure>

> 1. 如果您尚未创建任何细分，您可以访问[Contact](https://www.ycloud.com/console/#/app/contact/contactList)来添加细分。
> 2. 最多可**同时选择10个segment**。

当您遇到next无法点击时，说明campaign信息填写不完整。

请检查

1. 已选择至少1个segment

<figure><img src="../.gitbook/assets/campaign-step2-segment-next.png" alt=""><figcaption></figcaption></figure>

填写完毕后，点击next，进入步骤3



3.3.2 选择：联系人特征

单击联系人特征，可以根据联系人的属性/特征，筛选。

<figure><img src="../.gitbook/assets/campaign-step2-contactAttribute-null.png" alt=""><figcaption></figcaption></figure>

点击add filter，选择合适的筛选条件，进行过滤。

符合条件的，将成为本次campaign的收件人。

<figure><img src="../.gitbook/assets/campaign-step2-contactAttribute-selected.png" alt=""><figcaption></figcaption></figure>

&#x20;

## 步骤3: 设置变量

如果模板中有媒体头、变量，您可以在此步骤中设置这些值。 如果模板中没有变量，这部分不会显示，您可以按下一步继续。

### Headers（标头）

YCloud会提供默认的示例媒体配置文件，建议更改此媒体，以便更容易通过审核。

<figure><img src="../.gitbook/assets/image (649).png" alt=""><figcaption></figcaption></figure>

### Variables（变量）

如果模板中存在变量，请上传您的带变量的文件，然后手动将模板中的变量与文件中的变量值进行匹配。

<figure><img src="../.gitbook/assets/image (651).png" alt=""><figcaption></figcaption></figure>

将变量设置为固定值。选择Set a fixed text并为其指定一个值。

<figure><img src="../.gitbook/assets/image (652).png" alt=""><figcaption></figcaption></figure>

单击Next查看活动详细信息。



## 步骤4: 检查详细信息

确认详细信息并预览消息。\
确保您已点击Submit按钮以完成提交。

<figure><img src="../.gitbook/assets/image (653).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (654).png" alt=""><figcaption></figcaption></figure>

