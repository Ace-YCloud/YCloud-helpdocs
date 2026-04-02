---
description: 了解在 YCloud 如何管理联系人事件
---

# 联系人事件

## 事件的定义

跟踪 YCloud 中的事件可以让您更好地了解客户如何使用您的产品。这种理解使您能够发送有针对性的相关消息，并为您提供支持客户所需的所有上下文。

事件，代表您的客户做什么以及何时做的信息，例如：

* 当客户注册
* 当客户在网站上将商品加入购物车
* 当客户开始结算
* 当客户完成下单
* 当用户登记会员

事件可被用于 YCloud 平台下的多种产品模块：

* **在Journey中作为Trigger触发**
* 在Inbox里用于客服查看最近的用户互动
* 在CTWA作为转化结果定义

用于实现的用例：

* **Journey：一旦客户发生账单结算事件就进入流程，等待20分钟后发送WhatsApp营销消息催促客户完成付款，一旦客户发生下单事件就离开流程**
* Inbox：客服实时查看客户发生的关键动作
* CTWA：当客户下单成功，发生下单事件，作为本次CTWA的转化结果，传递给广告平台
* ……

{% hint style="info" %}
此处描述的事件只是示例，您可以根据自己的需求设计。
{% endhint %}



## 事件的属性

每个事件包含的信息包括：

* 事件名称
* 发生事件的时间
* 对象标识
* 联系人号码

您跟踪的每个事件也可以包含属性。这是有关事件的每个特定事件的其他信息。例如：如果您跟踪 “purchase” 事件，则元数据可以是所购买商品的名称和价格。

* `STRING`：长度不超过 255 个字符的纯字符串。
* `NUMBER`：最多具有一位小数的数值。
* `TIMESTAMP`：事件戳
* `URL`：格式为以`http://`或`https://`开头的字符串



## 创建和传递事件

默认情况下，YCloud 仅跟踪一些基础事件，例如您的Contact列表中新增联系人。

**更多有价值的事件往往需要工程师或开发人员的帮助才能实现，请将此文档发给您的同事，并告知他们你将如何使用它。**

创建事件定义：[https://docs.ycloud.com/reference/custom\_events-create-definition](https://docs.ycloud.com/reference/custom_events-create-definition)

发送事件：[https://docs.ycloud.com/reference/custom\_events-send-event](https://docs.ycloud.com/reference/custom_events-send-event)

