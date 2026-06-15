---
doc_id: doc_chatbot_chatbot_components_ask_a_question
language: zh-CN
title: "Ask a question"
slug: ask-a-question
path: chatbot/chatbot-components/ask-a-question
document_group: chatbot
path_in_group: chatbot-components/ask-a-question
parent_id: doc_chatbot_chatbot_components
order: 0
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T07:22:17.753Z
updated_at: 2026-04-02T07:22:17.753Z
last_synced_at: 2026-04-02T07:22:17.753Z
tags:
---

# Ask a question

## 什么是Ask a question?

Ask a question代表由商家端主动发起的提问，并且这个组件会等待用户回复信息，再对回复的内容进行后续的执行。



## Ask a question类型

* ### Text（文字形式）
  * 以文字形式呈现的问题。当用户回复了信息之后，可以把用户回复的信息储存为一个变量，用于后续对客户的回复。
  * _举例：您可以询问客户的姓名，然后把客户回复的姓名保存到客户信息中。在后续跟客户聊天时，再把这个姓名插入到聊天内容中。_

<figure><img src="../../.gitbook/assets/企业微信截图_aa0a1324-934a-476d-a875-6e4068d8c28c.jpg" alt=""><figcaption></figcaption></figure>

* ### Button：快速回复按钮（最多支持设置三个）
  * 您可以在询问中提示，可以给客户几个选项进行选择，客户点击选项后会自动的回复该选项，从而可以根据客户的选择进行不同的路由。
  * _举例：您可以问客户是想咨询价格还是产品，如果客户回复价格，自动给客户发一个报价文档。如果客户点击产品，给客户自动发送一个产品介绍。_

<figure><img src="../../.gitbook/assets/企业微信截图_8c998ecf-6a8c-4949-825a-57ff97aaff2c.jpg" alt=""><figcaption></figcaption></figure>

* ### List：菜单栏
  * 最多可以设置10个选项回复。适合企业想进行快速回复，但是快速回复按钮又受限的场景。也可以对用户的问题和需求做进一步的细分和回复。

<figure><img src="../../.gitbook/assets/企业微信截图_966e1baf-99ae-462f-a6c8-8d2ea4fb883b.jpg" alt=""><figcaption></figcaption></figure>



## 其他相关设置

### 设置仅收集一次用户回复

操作指引：\
登录YCloud后台 > Chatbot > Flow > Ask a question (选择List/button格式）> 打开Limit user to anwser once only按钮

当开启后，Chatbot只会收集一次用户在当前问题的回复。用户无法在一个问题里选择两次不同的选项，Flow会按照用户第一次选择的选项继续进行。

<figure><img src="../../.gitbook/assets/image (772).png" alt=""><figcaption></figcaption></figure>

### 在List message上添加描述

操作指引：\
登录YCloud后台 > Chatbot > Flow > Ask a question > 选择List格式 > 点击Add description添加描述

{% hint style="info" %}
请注意：描述限制在72个字符以内
{% endhint %}

<figure><img src="../../.gitbook/assets/image (773).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (774).png" alt=""><figcaption><p>在List按钮下添加描述</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (775).png" alt=""><figcaption><p>最终展示效果</p></figcaption></figure>
