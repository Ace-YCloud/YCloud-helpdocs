---
doc_id: doc_integrations_qu_dao_quan_qiu_duan_xin_ru_men
language: zh-CN
title: "入门"
slug: ru-men
path: integrations/qu-dao/quan-qiu-duan-xin/ru-men
document_group: integrations
path_in_group: qu-dao/quan-qiu-duan-xin/ru-men
parent_id: doc_integrations_qu_dao_quan_qiu_duan_xin
order: 10
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T11:15:59.645Z
updated_at: 2026-04-02T11:15:59.645Z
last_synced_at: 2026-04-02T11:15:59.645Z
tags:
---

# 入门

短消息/消息传递服务，通常缩写为 SMS，是移动电话和其他移动设备系统中的文本消息传递组件。\
作为最重要的消息传递渠道，SMS 几十年来一直以多种方式提供服务，例如个人通信、身份验证、营销和通知。

## 开始之前

**了解YCloud短信**：[YCloud支持200+国家短信，您可以在我们的官网](http://www.ycloud.com/price)查看国家和价格

**收费**：短信按分段计费。当短信中的字符超过1条短信的限制时，短信将被分割成多条短信发送，我们称之为分段。[您可以在此处](duan-xin-ji-chu-yuan-li.md)查看短信字符限制。

**什么样的短信是收费的？**&#x77ED;信状态为{未送达、已送达、处理中}时需付费。有关状态说明，请单击[此处](duan-xin-ji-chu-yuan-li.md)。

## 开始使用

在对接短信渠道前您需要先联系客服开通短信功能。

成功开通后在Integration（集成）中可以看到短信的导航。

<figure><img src="../../../.gitbook/assets/image (375).png" alt=""><figcaption></figcaption></figure>

## 试用账户需知

您应该了解一些限制：

* 试用账户仅支持发送短信至您注册的手机号码。
* 至于发件人ID，您只能使用YCloud默认的发件人ID。
* 您可以从[入门页面](https://www.ycloud.com/console/#/app/sms/getStarted)或 [API 文档](https://ycloud.readme.io/reference/sms-send)测试 SMS 。

&#x20;您可以随时通过充值的方式[升级您的帐户。](https://www.ycloud.com/console/#/app/payments/buyCredits)会解除使用限制。



## 选择您最喜欢的方式进行接入

1. [**HTTP API**](duan-xin-gong-neng/api-jie-kou.md)：使用我们的 REST API 可以更轻松、更快速地访问。
2. [**批量消息**](duan-xin-gong-neng/qun-fa-xiao-xi.md)：使用现成的工具手工批量群发。
3. [**SDK**](https://github.com/YCloud-CPaaS)：专为快速、轻松的集成而设计。
4. [**SMPP**](duan-xin-gong-neng/smpp.md)：支持与SMSC保持持续连接。请联系我们的客服获取 SMPP 帐户。



## 查看发送记录

[点击访问发送记录页面](https://www.ycloud.com/console/#/app/integrations/sms/analytics/logs)

<figure><img src="../../../.gitbook/assets/image (379).png" alt=""><figcaption></figcaption></figure>



