---
doc_id: doc_inbox_zhu_guan_zhi_nan
language: zh-CN
title: "主管指南"
slug: zhu-guan-zhi-nan
path: inbox/zhu-guan-zhi-nan
document_group: inbox
path_in_group: zhu-guan-zhi-nan
parent_id: doc_inbox
order: 0
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T07:23:13.000Z
updated_at: 2026-04-02T07:23:13.000Z
last_synced_at: 2026-04-02T07:23:13.000Z
tags:
---

# 主管指南

## 添加团队成员

### 步骤1: 邀请团队成员

1. 要邀请团队成员，请点击左下角的“账户头像” 依次选择 Settings > Users and teams >[Users](https://www.ycloud.com/console/#/app/settings/usersAndTeams) 点击页面中的 “Invite user”按钮。

<figure><img src="../.gitbook/assets/image (311).png" alt=""><figcaption></figcaption></figure>

2. 填写待邀请成员的基本信息，点击按钮 “Add”。系统将向该成员邮箱发送一封激活邮件。

<figure><img src="../.gitbook/assets/image (319).png" alt=""><figcaption></figcaption></figure>

### 步骤2: 团队成员接受邀请

成员找到对应激活邮件并点击按钮“激活账号”接受邀请，完成账号的激活。

<figure><img src="../.gitbook/assets/image (322).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
请注意，受邀请的用户无需通过YCloud官网新注册账号。
{% endhint %}

{% hint style="warning" %}
完成以上步骤后，团队成员即可登录YCloud后台，并在Inbox中查看消息。如需系统自动将会话分配给他，需在对应的WhatsApp号码 设置 > 分配规则 中添加该用户。
{% endhint %}



### 步骤3: 将接待人员加入团队

设置客服，并将客服加入团队，为后续的分配及转接创造便利。

详情参考[创建团队](../zhang-hu-guan-li/yong-hu-he-tuan-dui.md#chuang-jian-tuan-dui)



## Inbox设置

### 授权发起新会话

为了便于您管理号码权限，Inbox 下设 Authority 子菜单，该功能可控制用户使用该号码发起新会话的权限。

#### **操作介绍**

1. 点击【添加成员】按钮，搜索需要添加的成员或团队进行添加
2. 对于已添加的成员或团队，通过列表右侧的【移除】按钮进行单个移除，或点击左侧的复选框进行选中后批量删除
3. 通过右上方的搜索框可以通过用户名称或邮箱地址搜索成员
4. 对于在设置的【用户与团队】中新邀请加入的成员，系统将自动赋予他们租户下所有号码的新会话发起权限，如果您不希望部分用户拥有特定号码的新会话发起权限，可以在此处进行移除

#### **使用场景**

以下是部分可参考的使用场景：

1. 不希望销售人员拥有部分号码的主动发起会话权限，可将销售人员从授权列表中移除
2. 代表不同产品线的号码，由不同的员工负责，他们只对自己被分配的号码有发起新会话权限

<figure><img src="../.gitbook/assets/image (932).png" alt=""><figcaption></figcaption></figure>

### 基础分配规则配置

您可设置新会话自动分配基础规则，分为优先规则和次优先规则：

优先规则可选择上次接待分配，优先给之前为该客户服务的接待人员（当客服在线时）；或按客户归属分配，优先给负责该客户账号的指定接待人员。

次优先规则可选择不分配；或按顺序分配或负载均衡分配。

您可自由组合这些规则,以满足不同的客户服务需求,提高工作效率。

#### **步骤1: 进入目标号码的设置页面。**

入口：[WhatsApp accounts ](https://www.ycloud.com/console/#/app/dashboard/account)> Settings > Assignment

<figure><img src="../.gitbook/assets/image (312).png" alt=""><figcaption></figcaption></figure>

#### **步骤2：设置优先分配规则**

**优先分配规则>次优先分配规则。**&#x5F00;启优先分配规则按钮，会先执行优先分配规则。当无法满足优先分配规则时，才会执行次优先分配规则的设置。

都开启的情况下，优先分配规则的**选项优先级由上到下**

* 优先级 1：会话进线是会判断客户是否有Owner，有Owner的情况下会将此会话强制分配给该Owner
* 优先级2：会话会分配给上一个接待该会话的客服（前提是该客服在线）
* 优先级 3：指定会话给具体的某个客服、某个客服团队、某个 Chatbot 或未分配

<figure><img src="../.gitbook/assets/My_Photor_1760605072772.jpg" alt=""><figcaption></figcaption></figure>

### **高级分配规则配置**

高级分配规则对订阅 Pro 及以上版本的用户开放。\
点击【创建高级分配规则】按钮创建新的高级分配规则。

<figure><img src="../.gitbook/assets/My_Photor_1760605427516.jpg" alt=""><figcaption></figcaption></figure>

如果您在同一租户的其他号码中已配置过高级分配规则，并希望复用其中的部分逻辑，即可在出现的弹窗中选择对应的规则进行【复制】，复制按钮将把选中的规则复制到您的画布中成为草稿，方便您在其基础上继续修改调整。\
如果您希望从空白画布开始创建，则点击【从草稿开始】按钮，即可进入空白画布。

<figure><img src="../.gitbook/assets/image (934).png" alt=""><figcaption></figcaption></figure>

#### **高级分配工具箱**

点击模块后的加号节点即可选择条件模块或动作模块，或从左侧选择希望添加的模块，完成配置后进行连线。

<figure><img src="../.gitbook/assets/image (935).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (936).png" alt=""><figcaption></figcaption></figure>

#### Condition 条件模块

1. 点击添加条件按钮，可以从国家、语言、归属、最近接待在线客服、消息进线时间五种条件中选择需要的条件进行添加
2. 系统将根据您配置的顺序，从上到下对进线用户的各项条件进行判断，并进入第一个符合的分支并执行后续的分配动作。如果您在条件后未配置动作模块，用户会话将被转到【未分配】列表中
3. 国家：系统将根据用户手机区号自动判断其所属国家与地区，并根据您配置的国家进行条件匹配决定是否进入分支
4. 语言：系统将尝试判断用户所用的语言，成功判断后根据您配置的语言进行条件匹配决定是否进入分支
5. 归属：系统将自动判断进线用户是否已有归属，如果检测到有归属则进入该条件分支
6. 最近接待在线客服：系统将判断上一次接待该用户的客服是否在线，如在线则进入该条件分支
7. 消息进线时间：根据用户消息进线时间，与您设置的时间段进行匹配，符合条件的进入条件分支
8. 不满足任何您配置条件的进线会话，将进入【其他】条件分支

<figure><img src="../.gitbook/assets/image (937).png" alt=""><figcaption></figcaption></figure>

#### Agent takeover 坐席接管模块

1. 用户归属客服接管：将会话分配给用户归属的客服，无论其是否在在线
2. 最近接待在线客服接管：将会话分配给上一次接待过用户的客服，该客服在线
3. 自定义客服接管：根据您的需要自定义分配的客服
   1. 选择分配给特定客服，则将忽略其在线状态直接将会话分配给他
   2. 选择分配给一个团队，则将会话分配给该团队，并根据团队内部具体规则路由到具体客服
   3. 分配给 Chatbot，可选择配置好的 Chatbot
   4. 分配给未分配收件箱，会话将自动进入未分配收件箱

<figure><img src="../.gitbook/assets/My_Photor_1762235314600.jpg" alt=""><figcaption></figcaption></figure>

#### 画布配置、保存与编辑

1. 完成组件编辑后您可以拖动节点上的线条来连接这些模块，通过画布左下角的按钮您可以放大、缩小画布，或自动将画布调整为适当的大小，还可以对模块进行排列规整。
2. 完成所有配置后，点击右上角【检查】按钮来检查您的配置是否合规。
3. 系统将自动为该高级分配规则生成固定规则的名字，您可以在左上角修改它。
4. 完成检查后点击【保存】按钮保存您的设置。

<figure><img src="../.gitbook/assets/image (940).png" alt=""><figcaption></figcaption></figure>

5. 完成配置后回到高级配置列表页，点击【编辑】按钮可进入画布编辑规则。
6. 在您准备好之后，打开高级分配开关即可令其生效。

<figure><img src="../.gitbook/assets/My_Photor_1762235528194.jpg" alt=""><figcaption></figcaption></figure>

### **自动化规则配置**

在自动化规则页面设置Inbox的自动应答规则：包括：欢迎消息、新用户破冰、未分配会话的自动回复、接待人员未及时回复时的自动回复、自动关闭会话。

<figure><img src="../.gitbook/assets/image (325).png" alt=""><figcaption><p>通过右侧箭头展开或收起设置内容，通过开关开启或关闭功能</p></figcaption></figure>

* **欢迎消息：**&#x60A8;可以设置一条欢迎消息,在客户第一次打开对话时自动发送。
* **破冰提示：**&#x8FD9;是一组可自定义的可点击文本提示,出现在新用户首次的聊天窗口中。它有助于客户快速了解商家提供的服务或且可触发聊天机器人执行特定工作流程。
* **自动回复未分配的对话：**&#x5982;果对话尚未分配,可设置系统自动回复,确保及时响应客户。
* **超时自动回复：**&#x5982;果客户消息在指定时间内未得到接待人员的回复,系统会自动向客户发送一条消息。您可设置提醒消息发送的等待时间。
* **自动关闭对话：**&#x5982;果客户在设定时间内没有响应,系统会自动关闭该对话。您可设置自动关闭的时间。

详细设置请参考 [自动化](../whatsapp-accounts-zhang-hao-guan-li/shou-ji-hao-ma-guan-li/zi-dong-hua.md)

### 客户标签系统配置

进入Contct > Settings > [Tags](https://www.ycloud.com/console/#/app/contact/settings/tags) 管理系统标签

接待人员可以使用已定义好的标签更好的管理并筛选客户

<figure><img src="../.gitbook/assets/image (326).png" alt=""><figcaption></figcaption></figure>

### 快捷回复配置

进入Your preference > [Canned Response](https://www.ycloud.com/console/#/app/userSettings/cannedResponse) 配置账号共用的预置回复，接待人员在聊天中可以快速引用。

<figure><img src="../.gitbook/assets/image (329).png" alt=""><figcaption></figcaption></figure>

🎉🎉 恭喜你，已完成了团队Inbox的基础配置，当然您还可以基于工作时间配置更智能的聊天机器人接待流程。详细设置请参考ChatBot

## 查看实时报告

作为主管，您需要实时了解团队的接待情况，可以进入Inbox > [Analytics ](https://www.ycloud.com/console/#/app/inbox/analytics)查看实时数据统计。

详细指引请参考文档：[Inbox数据分析](inbox-shu-ju-fen-xi.md)

<figure><img src="../.gitbook/assets/image (330).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (332).png" alt=""><figcaption></figcaption></figure>
