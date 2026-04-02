---
doc_id: doc_journey_journey_zui_jia_shi_jian
language: zh-CN
title: "Journey最佳实践"
slug: journey-zui-jia-shi-jian
path: journey/journey-zui-jia-shi-jian
document_group: journey
path_in_group: journey-zui-jia-shi-jian
parent_id: doc_journey
order: 570
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T11:06:49.067Z
updated_at: 2026-04-02T11:06:49.067Z
last_synced_at: 2026-04-02T11:06:49.067Z
tags:
---

# Journey最佳实践

以下最佳实践是参考 YCloud Journey 编写的，我们将介绍如何通过它构建客户旅程。

这些用例仅用于参考，您需要根据自己的需求设计更有针对性、更个性化、更符合订阅者购买体验的自动化流程。

## 废弃Checkout自动化

这个Journey给您带来的好处

* 目标购物者是那些放弃了结账的购物者。
* 提供给他们相应的折扣，邀请它们回来继续结账，完成下单



### Trigger设置

**进入Trigger：**

* 何时发送：联系人事件\_客户开始Checkout。_联系人事件需要由您定义和传递给YCloud，详细请参考_ [_如何自定义联系人事件_](https://helpdocs.ycloud.com/help-center/v/zh/contact/lian-xi-ren-she-zhi/lian-xi-ren-shi-jian)
* 发件人：选择您已经创建的WhatsApp手机号码
* 受众：在本用例中一般不会做额外限制
* 是否过滤退订客户：建议勾选
* 客户触发限制：选择“客户只要满足了条件，每次都触发”

**退出Trigger：**

* 退出规则：联系人事件\_客户下单成功

**目标：**

* 目标：联系人事件\_客户下单成功

### 创建等待时间

新建组件 Wait ，并设置等待时间，再将 Trigger 与 Wait 两个组件连接。

这代表您最多等待客户多长时间去完成结账下单。

### 创建您的消息

使用您的消息在为客户创造紧迫感。常见示例包&#x62EC;_&#x6B64;优惠将于今天到期！_&#x6216;_这些产品正在快速售罄 - 赶快购买，以免售罄！_&#x60A8;也可以提供大幅折扣以激励他们完成订单

请记得在消息中添加回到结账地址的链接，让客户从您的消息中点击返回。





