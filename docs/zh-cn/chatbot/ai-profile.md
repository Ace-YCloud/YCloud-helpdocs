---
doc_id: doc_chatbot_ai_profile
language: zh-CN
title: "AI档案"
slug: ai-profile
path: chatbot/ai-profile
document_group: chatbot
path_in_group: ai-profile
parent_id: doc_chatbot
order: 620
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T11:12:10.659Z
updated_at: 2026-04-02T11:12:10.659Z
last_synced_at: 2026-04-02T11:12:10.659Z
tags:
---

# AI档案

## 选择 AI Agent 角色

创建一个 AI智能体，并选择你希望它成为的角色。

<figure><img src="../.gitbook/assets/screenshot@2x.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/screenshot@2x (1).png" alt=""><figcaption></figcaption></figure>

## 快速开始

我们已经预先设置好了所有基本配置。您可以直接在下方关联您的品牌信息，然后在右侧的预览界面与AI对话查看效果。如果您需要调整AI配置，可以点击右上角的“编辑”按钮进入配置编辑界面。

<figure><img src="../.gitbook/assets/screenshot@2x (2).png" alt=""><figcaption></figcaption></figure>

## 如何为 AI Agent 写好的提示词

一个好的提示可以显著提高你的AI智能体的效率和准确性。本指南介绍了如何为YCloud上的AI智能体编写好的提示。首先，你需要了解**指令、行动**以及其他**能力**是如何工作的：

| 说明            | 通过逐步工作程序和其他一般原则（如回退处理和边界）来指导**AI智能体的**整体行为。                                                  |
| ------------- | -------------------------------------------------------------------------------------------- |
| <p>操作<br></p> | 指导AI何时以及如何独立触发动作。动作可以中断指令。例如，对于“结束对话”这一操作，你可以写成“当用户表示满意且没有更多问题时”。这样，只要用户表现出这种意图，AI智能体就会结束对话。 |
| 流程、知识库和行动手册   | 它们作为AI智能体的技能库存在，智能体在回答用户问题时可按需调用。其中，Flows优先级最高，会首先被触发。                                       |

### Writing instructions

在这个模块你可以告诉 AI 工作时应该参考的大致工作流程、沟通语言风格、边界问题处理等等。我们建议将指引分解成几个部分：

<figure><img src="https://ycloudteam.feishu.cn/space/api/box/stream/download/asynccode/?code=OTc2MWRmZDYwMzg0Zjk4YmM4OTc0YTIxYjIwZDE3ZDFfWEJPZjZ3a1BNM3JyanJvelBFUEl5a0szZXZHVXl1aEhfVG9rZW46WFg2M2JSWTZnb0QzSjB4SldTb2N0eHIybjBkXzE3NzIyNjU1MDQ6MTc3MjI2OTEwNF9WNA" alt=""><figcaption></figcaption></figure>

| **提示词组成部分** | **它是做什么用的**                                                  | **示例**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| ----------- | ------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 工作程序        | <p>逐步告知AI智能体如何引导用户交互<br></p>                                 | <ol start="1"><li>类人问候语，礼貌热情地欢迎用户</li><li><p>了解需求</p><ol><li>询问他们的需求，例如 “你在找什么？”</li><li>简要确认他们的回复（例如，“收到👍”）</li><li>保持自然，不要连珠炮似地提问。</li></ol></li><li><p>提供快速价值</p><ol><li>根据他们的回答，突出一项符合其需求的关键益处。保持简短（最多1 - 2句话）。</li></ol></li><li><p>收集联系人（软过渡）</p><ol><li>在进行了一些信息交流后，可以说：如果你愿意，我可以给你发送更多细节。</li><li>询问用户信息，{{邮箱}}，{{昵称}}</li><li>确保你已询问了所有必要信息，且不询问超出必要范围的信息</li><li>让它自然些，一次只问一个问题</li><li>示例：对于电子邮件，你可以问“联系你的最佳邮箱是什么？”</li></ol></li><li><p>处理利息</p><ol><li><p>如果他们表现出浓厚兴趣，就问“您想预订演示还是与专家交流？”</p><ol><li>如果是 → 升级到人工客服</li><li>如果尚未准备好 → 保持乐于助人但不施加压力</li></ol></li></ol></li><li><p>关闭</p><ol><li>结束前：还有什么我可以帮您的吗？</li><li>如果否，请礼貌地感谢访客，例如“感谢来访，{{nick_name}}！😊”</li></ol></li></ol> |
| 上下文         | 通过描述AI代理与之交互的对象以及对话的主要目的，为其提供上下文信息。                          | <ol start="1"><li>您正在与一位正在了解我们产品或服务的人交谈。</li><li>你的目标是获取客户信息</li></ol>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| 角色与沟通风格     | 解释AI智能体应扮演的角色、应使用的语气以及应如何进行沟通。                               | <ol start="1"><li>你是一位热情、乐于助人且随和的销售向导，从不强求。</li><li>一次只问一个问题。保持回复简短、清晰且鼓舞人心。</li><li>回复要简短且口语化，最多两句话。</li></ol>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| 跟进处理        | 告诉AI智能体在对话中后续要做什么，例如等待多长时间以及如果用户不回复下一步该采取什么行动。               | 如果5分钟后没有回复，发送：“嗨，想确认一下你是否还在？”如果再过5分钟仍然没有回复，发送：“我现在先结束聊天了，但随时都可以提问！并结束对话。注意：当前计时器以分钟为单位计时，最长持续时间不超过60分钟                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| 回退处理        | 告知AI智能体在用户输入不明确、不完整或超出其能力范围时应如何应对                            | 如果您不理解用户的意图，首先尝试以友好的方式确认。如果仍然无法理解，请升级到人工客服。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| 边界          | <p>定义了AI智能体不应该<em>尝试的内容</em>（例如法律建议、医疗诊断、财务建议、股票查询等）<br></p> | <ul><li>切勿编造本说明中未涵盖的事实、流程、价格或政策。</li><li>除非有明确指示，否则请勿分享个人、财务或敏感信息。</li><li>坚守你的职责，不要越权行事或提供建议。</li><li>切勿分享假设、观点或承诺。</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |

### Writing actions prompts

在引导的基础上，你可以定义在某些特殊场景下触发的行动。在引导的工作流程以外，如果与用户的对话中出发了以下描述中的场景，那么 AI 也会根据你的提示要求进行行动。

<figure><img src="https://ycloudteam.feishu.cn/space/api/box/stream/download/asynccode/?code=NTkxMjcyMmFkY2Y5YThlNDhjNGFkZDY2NWNhMTE1ZjhfeXg1N1phTTdVOFNCdGdmNUhiUUE1QkNBWm1LRnRIUFpfVG9rZW46VUt5Q2I5S0NxbzhncUN4aGlFR2NtSUFlbmxlXzE3NzIyNjU1MDQ6MTc3MjI2OTEwNF9WNA" alt=""><figcaption></figcaption></figure>

对于每个行动，请描述：

* **何时**应该发生（条件）
* AI Agent应该做什么

| **行动**  | **你可以为提示词写些什么**                           | **示例**                                                                                |
| ------- | ----------------------------------------- | ------------------------------------------------------------------------------------- |
| 关闭对话    | 告知座席在何种情况下可以结束对话，以及结束对话时是否需要向用户发送通知消息。    | 联系人确认其问题已解决，无需进一步帮助。                                                                  |
| 升级到人工客服 | 指示AI在不同场景下转移到相应的座席或座席团队。                  | <ul><li>如果用户表示希望由人工客服提供服务，则转接至客服：John</li><li>如果用户希望获得有关退款请求的建议，请转接至团队：支持团队</li></ul> |
| 添加联系人标签 | 描述在哪些场景下应该为用户添加哪些相应的标签。                   | <ul><li>如果用户表现出强烈的购买意向，则添加联系人“购买意向”</li><li>如果用户对产品A表现出强烈兴趣，则添加联系人“产品A”</li></ul>     |
| 更新联系人属性 | 告知AI智能体何时更新联系人属性。此外，它还可以限制AI智能体仅更新某些特定属性。 | 当用户提及\{{Contact.Email\}}、\{{Contact.Order\_address\}}时更新它们。                           |

只有在启用时，行动才能独立触发。如果禁用某个特定行动，它仍可在指令中使用，但无法在指令之外独立触发。这意味着，虽然该操作在预定义指令或操作手册中仍然可用，但在重新启用之前，无法在其他上下文中激活。

### Using variables, hand off and contact tags

<figure><img src="https://ycloudteam.feishu.cn/space/api/box/stream/download/asynccode/?code=OWZhNjU2N2ZhMWM3ZjFhY2RmMDQ4NjdlZjU4OTIyNTVfZm9KQzh2cDY4amdVRjltREpzUGJ3WUdqUG9jNTZXU3NfVG9rZW46SnRvUmJDRTEyb1hJeTF4U2dpRWN4YnpCbjhmXzE3NzIyNjU1MDQ6MTc3MjI2OTEwNF9WNA" alt=""><figcaption></figcaption></figure>

**变量**

**什么是变量？**

变量允许您在AI提示中引用特定的联系人信息。可以将它们视为占位符，会自动填充真实的客户数据。

**它们是如何工作的？**

只要你需要提及联系人详细信息，如姓名、电子邮件、购买历史记录或你创建的任何自定义字段，就可以简单地在提示中添加变量。AI智能体能够智能地理解何时：

* 读取字段值（例如，"你好 \{{contact.name\}}"）
* 根据对话上下文更新字段（例如，在聊天过程中获取电话号码）
  * &#x20; 示例：“在对话过程中收集客户的\{{contact.phone\_number\}}。”

**交接**

<figure><img src="https://ycloudteam.feishu.cn/space/api/box/stream/download/asynccode/?code=YmU3NDZiM2EwODg1ODBiOWRkZWUxMDNjMGE2NWYwMmVfQ1RBTkFsTlJXMzEwZTdTSEUybWZXam4xYXdwTHFrVEhfVG9rZW46UlBEc2JqbnJybzB2T2l4Sm03Z2NITk5KbnhnXzE3NzIyNjU1MDQ6MTc3MjI2OTEwNF9WNA" alt=""><figcaption></figcaption></figure>

**什么是交接？**

转接功能允许您在需要时将对话从AI智能体升级到人工座席。可用选项：

* 分配给特定座席 - 路由到特定团队成员
* 分配给团队 - 路由到特定团队的任何可用成员
* 分配给负责人 - 路由到联系人指定的账户负责人
* 分配给上一处理人员 - 路由到之前协助过该联系人且现在可提供服务的座席

使用时机：为复杂咨询、敏感问题或AI无法解决请求时配置转接规则。

**添加联系人标签**

<figure><img src="https://ycloudteam.feishu.cn/space/api/box/stream/download/asynccode/?code=YWZkYjJjOGI2NzVlZDJlNmQyNzA3ZjM1ZDQwMGQzMjhfNE9IYzhYd0hyWVJGcmVJckZPa25BVjZlckJ4MWNzdnRfVG9rZW46UmxrZWJhWUF4b3VhSlB4MXdTRmNzYVZObndkXzE3NzIyNjU1MDQ6MTc3MjI2OTEwNF9WNA" alt=""><figcaption></figcaption></figure>

**什么是联系人标签？**

标签是您可以根据联系人的行为或对话内容自动应用于他们的标记。使用方法：选择在对话过程中满足特定条件时应用的特定标签。常见用例：

* 兴趣追踪：如果用户询问“产品A”，自动为其标记“感兴趣产品A”
* 问题分类：为联系人标记“计费问题”或“技术支持”标签
* 潜在客户资格认定：为潜在客户标记“热门潜在客户”或“需要跟进”

好处：标签可帮助您对联系人进行细分、触发自动化工作流程，并在未来的互动中提供更好的个性化服务。<br>
