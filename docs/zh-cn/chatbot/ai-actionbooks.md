---
doc_id: doc_chatbot_ai_actionbooks
language: zh-CN
title: "AI行动指南"
slug: ai-actionbooks
path: chatbot/ai-actionbooks
document_group: chatbot
path_in_group: ai-actionbooks
parent_id: doc_chatbot
order: 650
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

# AI行动指南

## 设置行动指南须知

为 AI配置可用的、好用的行动指南需要结合技术知识、面向流程的思维和团队协作：

**选择优化效果显著的流程：**&#x9996;先确定1 - 2个通过 AI自动化可以显著降低客服支持工作的任务流程，尤其是那些目前由人工团队处理的重复性高频任务。

**了解你的API需求：**&#x8BB8;多操作依赖于连接到API来获取或更新数据（即数据连接器）。确保你知道需要哪些API，它们返回什么，以及如何在行动指南中使用它们。

**跨职能协作：**&#x521B;建行动指南通常需要产品、工程或运营部门的意见，尤其是在构建或更新 API 时。就所需的工作流程进行清晰沟通，对于建立合适的系统至关重要。

**测试与迭代：**&#x6784;建有效的行动指南是一个迭代的过程。它包括测试各种指令、解决极端情况的问题，以及持续优化，以提高可靠性和最终用户体验。

了解并执行以上要点将帮助您构建更有效的行动指南。

## 创建与管理行动指南

访问路径：Chatbot-手册（Manuals）-行动指南，点击“创建新行动指南”按钮。

<figure><img src="../.gitbook/assets/image (849).png" alt=""><figcaption></figcaption></figure>

在创建完行动指南后，您可以在列表中管理这些行动指南，通过切换状态按钮改变其草稿、在线状态，或通过动作列表中的删除按钮删除特定的行动指南。

<figure><img src="../.gitbook/assets/image (850).png" alt=""><figcaption></figcaption></figure>

#### 设置行动指南的标题和触发条件

每个行动手册都应该有一个**标题** ，以便您找到它，以及触发条件的描述，用于告知AI何时触发它。这非常重要，这样AI才能在正确的时间触发它。这清楚地描述了AI应该使用该行动手册的情况，也可以指出AI不应该使用该行动手册的情况。

<figure><img src="../.gitbook/assets/image (851).png" alt=""><figcaption></figcaption></figure>

#### 添加指令

使用**指令**模块向AI输入指令。您可以让AI访问您的数据库，使用数据连接器，存储响应数据并回复用户。

使用段落编号来清晰区分步骤，例如1. Xxxx。2. Xxxxx...不要将多个步骤混在一起，因为这会降低AI响应的质量。

在说明中尽可能提供更多信息，任何未提供的信息都可能被AI错误推断。

每条指令都以动词开头。要清晰、简洁，并尽可能完整。长指令的可靠性较低，因此如有需要，可将每条指令拆分为多个步骤。

#### 使用系统内置动作

系统为 AI 提供内置动作，输入“/”唤起下拉菜单。

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

如果您希望AI在执行指令时引用知识库中的内容，可以使用“检索知识”动作来实现此效果。AI将在知识库中搜索内容，并将其与找到的材料相结合形成回答。

如果您希望AI在完成所有指令后主动结束对话，可以使用“结束对话”操作。

如果您希望在特定步骤中将对话转接给人工客服处理，可以在相应步骤中使用“转接”操作并选择具体的转接目标。

#### 使用数据连接器（Data connectors）

您可以使用已配置生效的数据连接器，让AI查询和更新外部数据，同时丰富AI的回答。只需输入“/”，然后在下拉框中选择您需要的数据连接器即可。

<figure><img src="../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

#### 预览您的行动指南并激活它

在右侧的预览窗口中测试已配置的行动指南，你可以根据AI的响应调整和优化你的配置。一切设置好后，你现在就可以点击右上角的“激活启用”，让这个行动手册生效了。

<figure><img src="../.gitbook/assets/image (852).png" alt=""><figcaption></figcaption></figure>
