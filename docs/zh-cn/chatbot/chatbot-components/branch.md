---
doc_id: doc_chatbot_chatbot_components_branch
language: zh-CN
title: "Branch"
slug: branch
path: chatbot/chatbot-components/branch
document_group: chatbot
path_in_group: chatbot-components/branch
parent_id: doc_chatbot_chatbot_components
order: 60
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T11:05:12.891Z
updated_at: 2026-04-02T11:05:12.891Z
last_synced_at: 2026-04-02T11:05:12.891Z
tags:
---

# Branch

## 什么是Branch？

Branch用于客户属性条件判断，不会对客户展示。企业可以通过添加判断组件，对不同属性的客户和情况进行多样化的回复。

在一个Branch中，可以设置多个“filter”，可以对满足不同条件的客户进行分流回复。



## 适用场景

### 用户属性判断

以下图的Chatbot为例，这是一个电商客户的退货场景。下图中设置了三个Branch:

1. 最近一次的购买记录是小于七天的
2. TAG是意向高的客户
3. 其他条件

当用户触发了Chatbot关键词，开启对话时，这个Chatbot会在发送第一条消息前先对该用户的属性进行一个判断。比如：\
当用户满足了条件一，Chatbot会给客户回复退货地址信息；当用户满足了条件二或者是条件三，则会匹配到另外一条连接客服的flow。

> 请注意：当用户满足了多个条件时，则会根据Branch的顺序，优先匹配第一个条件连接的flow继续进行对话。

<figure><img src="../../.gitbook/assets/企业微信截图_05f755b6-646c-4d7b-893d-b58c46e9f9ed.jpg" alt=""><figcaption></figcaption></figure>

