---
description: 本文主要介绍如何利用YCloud Journey来唤起Shopify订单弃购的用户的支付行为
---

# Shopify最佳实践

这个Journey给您带来的好处

* 目标受众是那些在支付页面，已经输入好了相关信息但最后关闭了支付页面，并未支付成功的用户。
* 邀请用户回来继续结账，完成下单

## 前提

正式创建Journey前，您需要创建一个带有Shopify支付链接的消息模版。

* 设置好模版内容
* 在Buttons中选择Call to action > Visit Website > Shopify link, 设置好后保存即可。

<figure><img src="../../../.gitbook/assets/image (788).png" alt=""><figcaption><p>带有Shopify支付链接的消息模版</p></figcaption></figure>

## Trigger设置

**进入Trigger：**

* 发送时间：Shopify events\_Shopify checkout created
* 发件人：选择您已经创建的WhatsApp手机号码
* 受众：在本用例中一般不会做额外限制
* 是否过滤退订客户：建议勾选
* 客户触发限制：选择Enter every time the person matches the rules （客户只要满足了条件，每次都触发）

**退出Trigger：**

* 退出规则：Shopify events\_Shopify order paid

**目标：**

* 本用例中不设置额外的目标

## 创建等待时间

新建组件 Wait ，并设置等待时间，再将 Trigger 与 Wait 两个组件连接。

这代表您最多等待客户多长时间去完成结账下单。

## 选择消息模版

选择提前预设好的带有Shopify支付链接的消息模版，并选择好模版中变量对应的属性。连接Wait组件，点击保存完成Journey创建。

<figure><img src="../../../.gitbook/assets/image (789).png" alt=""><figcaption><p>选择对应的变量的模版</p></figcaption></figure>
