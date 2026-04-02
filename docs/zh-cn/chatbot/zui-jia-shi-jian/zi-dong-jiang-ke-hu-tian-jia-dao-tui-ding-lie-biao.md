---
doc_id: doc_chatbot_zui_jia_shi_jian_zi_dong_jiang_ke_hu_tian_jia_dao_tui_ding_lie_biao
language: zh-CN
title: "自动将客户添加到退订列表"
slug: zi-dong-jiang-ke-hu-tian-jia-dao-tui-ding-lie-biao
path: chatbot/zui-jia-shi-jian/zi-dong-jiang-ke-hu-tian-jia-dao-tui-ding-lie-biao
document_group: chatbot
path_in_group: zui-jia-shi-jian/zi-dong-jiang-ke-hu-tian-jia-dao-tui-ding-lie-biao
parent_id: doc_chatbot_zui_jia_shi_jian
order: 10
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T11:12:51.181Z
updated_at: 2026-04-02T11:12:51.181Z
last_synced_at: 2026-04-02T11:12:51.181Z
tags:
---

# 自动将客户添加到退订列表

{% hint style="info" %}
通过YCloud Chatbot自动识别客户退订意图，允许客户退订并自动加入退订列表，避免客户直接在向WhatsApp发起投诉。将有效避免WhatsApp账号被禁用。
{% endhint %}



示例：

当接收到客户要退订的消息时，Chatbot自动询问客户是否确认要退订，对于二次确认了退订的客户执行加入退订列表。

<figure><img src="../../.gitbook/assets/企业微信截图_780aa2cb-88ef-45c2-8a9d-fd93f2baebe5 (1).jpg" alt=""><figcaption></figcaption></figure>



## 步骤1: 登陆YCloud账号，创建Chatbot Flow

<figure><img src="../../.gitbook/assets/企业微信截图_e14b84bb-d55e-4eff-8225-5e0228f64e28.jpg" alt=""><figcaption></figcaption></figure>



## 步骤2: 添加退订的触发关键词

{% hint style="info" %}
建议：设置多个退订关键词，并且选择Containing(包含）而非 Exact matching(完全匹配)。这样，命中列表中的任意一个关键词都会触发Chatbot。设置完成后点击保存按钮。
{% endhint %}

<figure><img src="../../.gitbook/assets/企业微信截图_fbb477cd-1720-475a-bc8c-b8275c64b322 (1).jpg" alt=""><figcaption></figcaption></figure>



## 步骤3: 确认客户退订意愿的消息（可选）



{% hint style="warning" %}
强烈建议加入此步骤，以免客户误入退订列表。您可以选择使用Ask a question组件，询问客户：请您确认是否要退订消息？
{% endhint %}

详细步骤：

1. 选择Ask a question 组件

<figure><img src="../../.gitbook/assets/企业微信截图_029d54a3-5b72-4932-ac6a-20391a58b8db.jpg" alt=""><figcaption></figcaption></figure>

2. 选择Buttons的消息形式

<figure><img src="../../.gitbook/assets/企业微信截图_c1952858-e095-407c-847e-717e93d36c2f.jpg" alt=""><figcaption></figcaption></figure>

3. 设置询问内容：请您确认是否要退订消息？

* 设置Button的两个选择
  * 是的，我要退订你们的消息
  * 不，我点错了
* 设置完成后点击Save

<figure><img src="../../.gitbook/assets/企业微信截图_a5594dda-aaf9-42fa-974d-119f0a756367.jpg" alt=""><figcaption></figcaption></figure>

4. 设置完成后连接 Keyword trigger 到 Ask a question 组件

<figure><img src="../../.gitbook/assets/企业微信截图_05a33704-b15c-44a9-9dd9-d7a7d6a14440.jpg" alt=""><figcaption></figcaption></figure>



## 步骤4: 加入退订列表

1. 加入退订组件

<figure><img src="../../.gitbook/assets/企业微信截图_ae8f457b-5225-46e1-9e2d-def540be66d9.jpg" alt=""><figcaption></figcaption></figure>

2. 可以选择是否要自动回复退订成功。如果需要添加自动回复，点击Auto-reply右侧开关，并在下方输入自动回复内容，选择Save进行保存。

<figure><img src="../../.gitbook/assets/企业微信截图_74afd5cd-365d-4b7d-bf49-16999b0e0489.jpg" alt=""><figcaption></figcaption></figure>

3. 将 Ask a question 组件中的 【是的，我要退订】按钮连接到退订组件

<figure><img src="../../.gitbook/assets/企业微信截图_be99b646-95be-44bd-9e99-f910e494a17e.jpg" alt=""><figcaption></figcaption></figure>



## 步骤5: 增加发送文本（可选）

增加一个Send messages 文本组件，并连接到【不，我点错了】按钮

<figure><img src="../../.gitbook/assets/企业微信截图_d28fac25-2206-4737-ab7f-43dab011b10b.jpg" alt=""><figcaption></figcaption></figure>



## 步骤6: 保存Chatbot并启用

编辑好Chatbot模版后，点击右上角的Save，并且在弹窗内点击Active > Save，即刻完成退订Chatbot的激活。当客户触发退订关键词，Chatbot会自动将此号码加入退订名单，并且显示在 Contact > Unsubscribe 的名单里。

<figure><img src="../../.gitbook/assets/企业微信截图_46800f98-617f-4e77-91eb-ec4a02b099ff.jpg" alt=""><figcaption></figcaption></figure>
