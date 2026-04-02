---
description: Marketing Messages Lite API
---

# MM Lite API

Marketing message Lite API（“简称MM Lite API ”）是Meta最新推出的发送WhatsApp 营销模板消息的接口。



## 怎样的企业适合使用此接口？

有营销需求的企业。



## 用MM Lite API 发送有什么好处？

✅  对于比Cloud api（您当前在使用YCloud平台发出的消息均由Cloud api发送），MM Lite API有更高的达到率和阅读率。通过MM lite API 发送的营销消息会经过Meta的AI系统，此系统会帮助您触达活动中更偏好收取营销消息的客户，从而来提高营销活动的表现效果。

✅ 通过MM Lite API 发送的消息会在您的广告系统中看到数据，若您已经在网站中使用了Pixel埋点，可以在广告账户中追踪营销消息的效果。

✅ 开启了MM Lite API的 WhatsApp business account 支持给营销模板设置消息的有效时间。



## 如何使用?

只需要对WABA（WhatsApp business account）进行重新授权，即可开通MM Lite API。

开启后，所有从已授权的WABA中发出的营销模板消息，均会自动通过MM Lite API进行发送（不支持MM Lite API 触达的地区会YCloud自动转为Cloud api进行发送）。

访问 [MM Lite API 授权页面](https://www.ycloud.com/console/#/app/integrations/mmLiteApi)， 点击 **授权** 按钮。在弹窗中选需要授权的WABA，并完成授权流程。

{% hint style="info" %}
注意，在授权时，您必须是此WABA的管理员。
{% endhint %}

<figure><img src="../.gitbook/assets/image (50).png" alt=""><figcaption></figcaption></figure>



## MM Lite API 功能的地理可用性

由于 Meta 的政策以及各国的法律法规，MM Lite API 的某些高级功能和数据报告能力仅在特定地区可用，不同地区对功能的支持情况有所不同。





### 美国

• 从 2025 年 4 月 1 日起，所有发送给美国 WhatsApp 用户的营销消息将不会被递送，Meta 将直接拦截这些消息，并返回错误代码 131049。

• 需要注意的是，这一政策并不仅限于 MM Lite API，而是适用于所有 WhatsApp 业务消息 API，包括 Cloud API（云 API）。

• 美国的企业号码仍然可以向美国以外的 WhatsApp 用户发送消息，但无法向美国本土用户发送营销类消息。



### 古巴、伊朗、朝鲜、叙利亚，以及乌克兰的克里米亚、顿涅茨克、卢甘斯克地区

• 这些地区的企业无法开通 WhatsApp 业务 API 账号。

• 任何 WhatsApp 业务账号无法向这些地区的用户发送消息，无论是营销消息还是其他类型的消息。

• 这项政策不仅适用于 MM Lite API，也适用于所有 WhatsApp 业务消息 API（包括 Cloud API）。

##
