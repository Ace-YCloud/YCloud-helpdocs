# 通过WhatsApp发送通知消息

{% hint style="info" %}
通过WhatsApp发送通知类型消息具有明显的优势，包括有保证的交付，更高的读取率和响应率，以及直接在对话中采取行动的能力。
{% endhint %}



## 1. 创建WhatsApp消息模版

* 登录YCloud后台，[点击访问](https://www.ycloud.com/console/#/entry/login?lastPath=https%3A%2F%2Fwww.ycloud.com%2Fconsole%2F%23%2Fapp%2Fdashboard%2FgetStarted)
* 点击Home > Templates >  + Add Template

<figure><img src="../.gitbook/assets/image (274).png" alt=""><figcaption></figcaption></figure>

* 在Category选择Utility，并命名模版名称和选择模版语言
  * 请注意：**模版名称必须要唯一的**。名称仅支持小写字母a-z、0-9、 下划线（\_)。模版一旦提交，无法进行更改。

<figure><img src="../.gitbook/assets/image (293).png" alt=""><figcaption></figcaption></figure>

* 输入要发送的内容

{% hint style="warning" %}
请注意：通知类消息用于发送帐户更新、订单更新、警报和其他重要信息，包括但不仅限于：

* 更改/更新交易：i.e.: Your password has changed/ Your order has been dispatched
* 账户/账单/付款通知：i.e.: Your payment has been accepted/ Your payment has failed
{% endhint %}

<figure><img src="../.gitbook/assets/image (295).png" alt=""><figcaption></figcaption></figure>

* 点击提交（Submit) & 等待审核通过
  * 如果模版没有通过，可以[申请复审](https://business.facebook.com/accountquality/)



## 2. 发送通知消息

* ### 通过群发工具（Campaign）发送

{% hint style="info" %}
点击查看超详细教程
{% endhint %}

* 访问YCloud后台，[点击访问](https://www.ycloud.com/console/?redirect=/edit/getting-started#/app/dashboard/getStarted)&#x20;
* 如下图，点击+ Add campaign创建发送

<figure><img src="../.gitbook/assets/image (296).png" alt=""><figcaption></figcaption></figure>



* ### 通过API发送通知消息

{% hint style="info" %}
点击查看[API发送消息接口地址](https://docs.ycloud.com/reference/whatsapp_message-send)
{% endhint %}



## 常见问题

