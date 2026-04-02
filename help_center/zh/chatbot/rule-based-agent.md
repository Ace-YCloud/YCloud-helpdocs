---
description: 不含AI，简单明确的基于工作流的机器人，适用于固定流程的任务
---

# 规则机器人

## 什么是规则机器人

如果您的业务需求可以通过简单的工作流程来满足，基于规则的智能体是一个绝佳选择。它不包含AI组件，仅通过关键词或消息按钮触发聊天机器人的响应来运行。此外，您还可以配置其基本设置，如欢迎消息、自动关闭会话时间和兜底行为。

<figure><img src="../.gitbook/assets/image (33).png" alt=""><figcaption></figcaption></figure>

## 如何配置一个规则机器人

<figure><img src="../.gitbook/assets/image (34).png" alt=""><figcaption></figcaption></figure>

#### 档案（Profile）

**头像和名称**

你可以根据需要设置规则机器人的头像和名称

<figure><img src="../.gitbook/assets/image (35).png" alt=""><figcaption></figcaption></figure>

**当它不理解用户意图的时候应该怎么做（兜底行为）**

可以配置规则机器人的兜底行为：

1. 保持无回应。机器人不会下发任何消息。
2. 自动回复。可以配置自动回复，机器人在不理解用户意图时发送配置的回复内容。
3. 转接人工。选择该选项，机器人在不理解时会将会话转接给人工客服处理。

**机器人应该等待多久后自动关闭会话**

当 Chatbot 下发消息后，用户如果在配置时间内完全没有任何回复，那么机器人将主动关闭会话。具体等待时长支持配置，默认为 10 分钟。

**会话开始时的欢迎消息**

机器人的欢迎消息是在其处理的每次对话开始时发送给用户的自动消息。您可以在此处配置一些您希望用户在收到消息后立即看到的消息，支持纯文本、媒体或交互式消息类型。

<figure><img src="../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>

#### [流程（Flows）](chuang-jian-yi-ge-flow.md)

通过创建流程来规定 Chatbot 与用户的具体交互流程，完成简单明了的工作流任务。
