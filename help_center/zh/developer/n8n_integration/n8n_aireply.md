---
hidden: true
---

# 最佳实践：AI自动回复

本示例将演示如何通过 n8n + 大语言模型实现一个基础的自动回复流程：

当 YCloud 收到 inbound message 后，通过 Webhook 触发 n8n 工作流，调用大模型生成回复内容，并通过 YCloud API 将消息返回给用户。

> YCloud Chatbot 为您构建了完整的AI工作流，提供全链路简单易懂的AI知识库，语料，自动化流程。您可以[点此链接](/broken/pages/PhbyQBXo6pcfsOKRwZ6O)查看详情。

***

### 总体流程

<figure><img src="../../.gitbook/assets/image (2) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

### Webhook 事件触发

设置Webhook事件中，请将HTTP Method设置为POST，Response为立即返回，且返回状态码为200。

{% hint style="info" %}
请注意保护好您的Webhook URL，且勿必只返回**状态码200**。
{% endhint %}

<figure><img src="../../.gitbook/assets/image (3) (1) (1).png" alt=""><figcaption></figcaption></figure>

您需要在YCloud Webhook event中选择 WhatsApp.inbound\_message.received。 当 YCloud Webhook 被触发后，n8n 的 Webhook 节点会接收到完整的 inbound\_message 数据，并自动解析为可用字段。如下图所示：

<figure><img src="../../.gitbook/assets/image (4) (1).png" alt=""><figcaption></figcaption></figure>

这些字段将作为后续节点（Data Table、AI Agent、HTTP Request 等）的输入数据，可通过 Expression 方式进行引用。

***

### Data Table 操作

#### Data Table 表设计

您可以完全依照Webhook推送的字段来进行设计。如wamid, from, name, to, sendtime, type等。这些字段被保留，能防止回复重复的问题。

#### Insert Row

该节点用于将 Webhook 接收到的数据写入 Data Table，用于后续查询或状态管理。

* 支持 手动匹配 或 自动匹配
* 自动匹配要求字段名称完全一致
* 可直接将 Input 面板中的字段拖入配置项，n8n 会自动生成 Expression

<figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

#### Get Row

该节点用于从 Data Table 中读取已存在的数据。

<figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

在该节点中，通常需要配置 匹配条件（Condition），例如：

* 使用 Webhook 中的 wamid
* 与 Data Table 中已存储的 wamid 字段进行匹配

该方式常用于判断消息是否已处理，或读取历史上下文。

***

### AI Agent 操作

#### 1. 配置模型

在使用 AI Agent 之前，请先在 Credentials 中配置对应的模型信息（如 OpenRouter, ollama 等）。在本节中，将使用OpenRouter进行配置。

此处Credential不进行截图配置，使用来自OpenRouter的相关API即可。您可以选择您想要的模型与返回格式，在此最佳实践中选择grok-3与TXT格式。

<figure><img src="../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

***

#### 2. AI Agent 节点

在 AI Agent 节点中：

* 编写 Prompt
* 使用 Expression 引用 Webhook 或 Data Table 中的字段作为输入。您可以编写您想要的Prompt，此处不进行添加。Prompt 内容可根据业务需求自由定制。

<figure><img src="../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

您可以选择不同的工具来接入AI Agent节点，将其与节点相连即可。

<figure><img src="../../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>



> 说明：AI Agent 支持扩展记忆机制（Memory），可通过数据库或其他存储方式实现上下文管理。

您可以在此处看到模型最终输出的信息。

<figure><img src="../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

***

### Merge 操作

Merge 节点用于合并多个节点的输出数据，为后续 API 请求做准备。

<figure><img src="../../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

常见模式包括：

* Append
* Combine
* Merge by Index

在当前示例中，使用合并模式将多个输出拼接为一个数据结构，供 HTTP Request 节点使用。

***

### HTTP Request（发送回复消息）

最后，通过 HTTP Request 节点调用 YCloud 消息发送接口。

<figure><img src="../../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

* 可直接使用 YCloud API 文档中的 cURL 示例 进行快速配置，将APIkey插入 X-API-KEY所对应的位置。
* 将上一步合并后的字段拖入请求体中

{% hint style="warning" %}
此处请务必注意消息发送方与接收方为**反向**，此处为回复消息。
{% endhint %}

* 使用 Expression 表达式动态填充消息内容、接收方等参数

至此，一个完整的 Webhook → 大语言模型 → 自动回复 的n8n流程即配置完成。

***

### 小结

通过以上步骤，你可以快速构建一个基于 n8n 的自动回复工作流，实现：

* Webhook 监听
* 消息数据处理
* LLM 自动生成内容
* 通过 YCloud API 回复用户

该示例作为通过n8n集成的起点。

