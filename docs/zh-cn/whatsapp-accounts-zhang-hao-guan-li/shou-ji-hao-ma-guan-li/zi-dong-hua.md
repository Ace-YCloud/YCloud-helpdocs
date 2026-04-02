---
doc_id: doc_whatsapp_accounts_zhang_hao_guan_li_shou_ji_hao_ma_guan_li_zi_dong_hua
language: zh-CN
title: "自动化"
slug: zi-dong-hua
path: whatsapp-accounts-zhang-hao-guan-li/shou-ji-hao-ma-guan-li/zi-dong-hua
document_group: whatsapp-accounts-zhang-hao-guan-li
path_in_group: shou-ji-hao-ma-guan-li/zi-dong-hua
parent_id: doc_whatsapp_accounts_zhang_hao_guan_li_shou_ji_hao_ma_guan_li
order: 40
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T11:19:00.741Z
updated_at: 2026-04-02T11:19:00.741Z
last_synced_at: 2026-04-02T11:19:00.741Z
tags:
---

# 自动化

自动化是针对号码的配置项，包含：

* [welcome message](zi-dong-hua.md#welcome-message-huan-ying-xiao-xi-yi-xia-xian): 欢迎消息（已下线）
* [Ice breaker](zi-dong-hua.md#ice-breakers-po-bing-ti-shi)：破冰提示。
* [Auto-reply for unassigned conversation](zi-dong-hua.md#autoreply-for-unassigned-conversations-zi-dong-hui-fu-wei-fen-pei-dui-hua)：自动回复未分配对话。
* [Auto-reply for delayed agent responses](zi-dong-hua.md#autoreply-for-delayed-agent-responses-chao-shi-zi-dong-hui-fu)：超时自动回复。
* [Auto-reply for in queue conversations:](https://helpdocs.ycloud.com/help-center/v/zh/whatsapp-accounts-zhang-hao-guan-li/shou-ji-hao-ma-guan-li/zi-dong-hua#autoreply-for-in-queue-conversations-zi-dong-hui-fu-zai-pai-dui-zhong-de-hui-hua) 自动回复正在等待中的会话。
* [Auto-close Inbox conversations](zi-dong-hua.md#autoclose-inbox-conversations-chao-shi-zi-dong-guan-bi-dui-hua)：超时自动关闭对话。
* [CSAT](https://helpdocs.ycloud.com/help-center/v/zh/whatsapp-accounts-zhang-hao-guan-li/shou-ji-hao-ma-guan-li/zi-dong-hua#csat-man-yi-du-diao-cha-wen-juan)：自动发送满意度调查问卷。

自动化的设置入口：Home > WhatsApp accounts > 号码的Settings > Automation

<figure><img src="../../.gitbook/assets/image (302).png" alt=""><figcaption><p>Automations</p></figcaption></figure>

##

## Welcome message（欢迎消息）- 已下线

**发送时机**：每当 WhatsApp 用户首次与您打开聊天窗口时。

{% hint style="info" %}
注意：是当客户首次打开跟您的聊天窗口时触发，他可能还未发送任何消息给您。
{% endhint %}

<figure><img src="../../.gitbook/assets/image (303).png" alt=""><figcaption><p>Welcome message</p></figcaption></figure>

**发送的消息格式**：欢迎消息可发送自由格式的消息：文本、图文、带按钮的互动类消息。_例如：图文消息，可查看以下示例：_

<figure><img src="../../.gitbook/assets/image (304).png" alt=""><figcaption><p>Media message as Welcome message</p></figcaption></figure>

**使用场景**：欢迎消息非常适合服务互动，例如客户支持。例如，您可以在应用或网站上嵌入 WhatsApp 按钮。当用户点击该按钮时，他们将被引导到 WhatsApp，在那里他们将收到一条欢迎消息，其中提供了有关如何与您互动的背景信息。

**收费**：欢迎消息虽是商家主动发送的消息，但发送的消息将收取服务对话类型费用。

### 操作步骤

#### 步骤1：开启欢迎消息开关

<figure><img src="../../.gitbook/assets/image (305).png" alt=""><figcaption><p>Enable welcome message</p></figcaption></figure>

#### 步骤2：编辑自动回复的消息内容

发送的消息类型支持以下3种：

* 文本消息：纯文字类型消息。支持Emoji，加粗，斜体等样式。
* 富媒体消息。图片/视频/文件 + 文字类型的消息。
* 互动类消息。带按钮的互动消息，如快捷回复按钮、跳转按钮、列表按钮。

{% hint style="info" %}
注意：互动类消息中，如果您想使用列表按钮，Header务必设置为None或者纯文本Header。
{% endhint %}

<figure><img src="../../.gitbook/assets/image (306).png" alt=""><figcaption><p>Save welcome message</p></figcaption></figure>



## Ice breakers（破冰提示）

破冰提示为用户提供了一种通过常见问题列表与企业展开对话的方式。当用户打开您的对话窗口时，在用户的输入框内会出现一列预置的破冰语，用户点击后会立即发送消息。

<figure><img src="../../.gitbook/assets/image (307).png" alt=""><figcaption><p>Ice breakers</p></figcaption></figure>

**规则**：您最多可以在一个电话号码上配置 4 个破冰提示。每个破冰游戏最多可以有 80 个字符。不支持表情符号。

### 操作步骤

#### 步骤1：开启破冰提示开关

<figure><img src="../../.gitbook/assets/image (308).png" alt=""><figcaption><p>Enable ice breaker</p></figcaption></figure>

#### 步骤2：设置选项

设置完选项后点击保存。

<figure><img src="../../.gitbook/assets/image (309).png" alt=""><figcaption><p>Edit and save Ice breaker</p></figcaption></figure>

## Auto-reply for unassigned conversations（自动回复未分配对话）

当进入对话未分配，即无人接待时，系统自动给客户回复一条消息，确保及时响应客户。

<figure><img src="../../.gitbook/assets/image (321).png" alt=""><figcaption><p>Auto-reply for unassigned message</p></figcaption></figure>

### 操作步骤

#### 步骤1：打开开关

<figure><img src="../../.gitbook/assets/image (310).png" alt=""><figcaption><p>Enable auto-reply for unassigned conversations</p></figcaption></figure>

#### 步骤2：编辑自动回复内容

点击Edit按钮进行编辑。发送的消息类型支持以下3种：

* 文本消息：纯文字类型消息。支持Emoji，加粗，斜体等样式。
* 富媒体消息。图片/视频/文件 + 文字类型的消息。
* 互动类消息。带按钮的互动消息，如快捷回复按钮、跳转按钮、列表按钮。

设置完成后点击保存。

<figure><img src="../../.gitbook/assets/image (320).png" alt=""><figcaption><p>Edit and save auto-reply for unassigned conversations</p></figcaption></figure>

## Auto-reply for in queue conversations（自动回复在排队中的会话）

当打开这个开关后，在排队中的会话会收到一条自动发送的消息，通知客户目前处于等待接待的状态，来保证回复的实效性。

如果当前接待人员已到达接待上限人数后，关闭了其中一个会话，在队列中排队的会话会自动进入到接待人员的收件箱中。



另外，接待人员也可以手动去认领在排队中的会话。

### 操作步骤

**方法一：**

当当前到达接待会话上限时，接待人员的Inbox界面上方会显示当前正在排队的人数。点击 people in queue，勾选想要转接给自己的会话，即可转接成功。

<figure><img src="../../.gitbook/assets/image (651).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (652).png" alt=""><figcaption></figcaption></figure>

**方法二：**

Inbox > Unassigned > In queue

可以看到正在排队中的会话，点进会话后进行会话转接。

<figure><img src="../../.gitbook/assets/image (654).png" alt=""><figcaption></figcaption></figure>

## Auto-reply for delayed agent responses（超时自动回复）

如果客户消息在指定时间内未得到接待人员的回复，系统会自动向客户发送一条消息。您可设置提醒消息发送的等待时间。

### 操作步骤

#### 步骤1：打开开关

<figure><img src="../../.gitbook/assets/image (322).png" alt=""><figcaption><p>Enable Auto-reply for delayed agent responses</p></figcaption></figure>

#### 步骤2：设置等待时间和回复内容

等待时间：当接待人在设置的时间内仍然未回复客户，系统会自动回复消息。

点击Edit按钮进行内容编辑。发送的消息类型支持以下3种：

* 文本消息：纯文字类型消息。支持Emoji，加粗，斜体等样式。
* 富媒体消息。图片/视频/文件 + 文字类型的消息。
* 互动类消息。带按钮的互动消息，如快捷回复按钮、跳转按钮、列表按钮。

设置完成后点击保存。

<figure><img src="../../.gitbook/assets/image (323).png" alt=""><figcaption><p>Edit and save Auto-reply for delayed agent responses</p></figcaption></figure>

## Auto-close Inbox conversations（超时自动关闭对话）

在人工接待的情况下，客户在设定时间内没有回复任何消息, 系统会自动关闭该对话。您可设置自动关闭的时间。

{% hint style="info" %}
此设置项对未分配的对话，和分配给机器人的对话不生效。为分配的对话不会自动关闭，分配给机器人的对话有两种关闭方式：

1. 执行完流程后关闭对话。
2. 客户未响应机器人10分钟后关闭。
{% endhint %}

### 操作步骤

#### 步骤1：开启开关

<figure><img src="../../.gitbook/assets/image (324).png" alt=""><figcaption><p>Enable auto-close Inbox conversation</p></figcaption></figure>

#### 步骤2：编辑自动关闭时间

支持配置范围：1分钟\~72小时。

建议配置参数：24小时。

配置完成后点击保存。

<figure><img src="../../.gitbook/assets/image (325).png" alt=""><figcaption><p>Save auto-close Inbox conversations</p></figcaption></figure>

## CSAT (满意度调查问卷）

当打开了这个开关之后，由人工接待的会话结束之后，会自动给用户发送一条满意度调查的信息。请注意，如果是由BOT接待的会话，不会触发满意度调查问卷。**该功能仅对于人工接待的会话有效。**

### 操作步骤

#### 步骤1：开启开关

<figure><img src="../../.gitbook/assets/image (655).png" alt=""><figcaption></figcaption></figure>

#### 步骤2：编辑文案

如下图，支持配置发送消息的文案和按钮文字。展开按钮后，调查问卷的格式为固定格式，无法进行修改。

<figure><img src="../../.gitbook/assets/image (656).png" alt=""><figcaption></figcaption></figure>
