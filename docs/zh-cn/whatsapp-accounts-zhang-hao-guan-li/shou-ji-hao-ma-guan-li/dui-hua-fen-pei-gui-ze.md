---
doc_id: doc_whatsapp_accounts_zhang_hao_guan_li_shou_ji_hao_ma_guan_li_dui_hua_fen_pei_gui_ze
language: zh-CN
title: "对话分配规则"
slug: dui-hua-fen-pei-gui-ze
path: whatsapp-accounts-zhang-hao-guan-li/shou-ji-hao-ma-guan-li/dui-hua-fen-pei-gui-ze
document_group: whatsapp-accounts-zhang-hao-guan-li
path_in_group: shou-ji-hao-ma-guan-li/dui-hua-fen-pei-gui-ze
parent_id: doc_whatsapp_accounts_zhang_hao_guan_li_shou_ji_hao_ma_guan_li
order: 30
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T11:19:00.741Z
updated_at: 2026-04-02T11:19:00.741Z
last_synced_at: 2026-04-02T11:19:00.741Z
tags:
---

# 对话分配规则

YCloud会将绑定的号码收到的新对话分配到Inbox（收件箱）中。此功能即针对Inbox中收到的新对话进行分配规则的设置。

## 入口

Home > WhatsApp accounts > 号码的Settings > Assignment

<figure><img src="../../.gitbook/assets/image (858).png" alt=""><figcaption></figcaption></figure>

## Basic Assignment（基础分配规则）

**优先分配规则>次优先分配规则。**&#x5F00;启优先分配规则按钮，会先执行优先分配规则。当无法满足优先分配规则时，才会执行次优先分配规则的设置。

都开启的情况下，优先分配规则的**选项优先级由上到下**

* 优先级 1：会话进线是会判断客户是否有Owner，有Owner的情况下会将此会话强制分配给该Owner
* 优先级2：会话会分配给上一个接待该会话的客服（前提是该客服在线）
* 优先级 3：指定会话给具体的某个客服、某个客服团队、某个 Chatbot 或未分配

<figure><img src="../../.gitbook/assets/image (859).png" alt=""><figcaption></figcaption></figure>

## Advanced Assignment（高级规则）

高级分配规则对订阅 Pro 及以上版本的用户开放。\
点击【创建高级分配规则】按钮创建新的高级分配规则。

<figure><img src="../../.gitbook/assets/image (861).png" alt=""><figcaption></figcaption></figure>

如果您在同一租户的其他号码中已配置过高级分配规则，并希望复用其中的部分逻辑，即可在出现的弹窗中选择对应的规则进行【复制】，复制按钮将把选中的规则复制到您的画布中成为草稿，方便您在其基础上继续修改调整。 如果您希望从空白画布开始创建，则点击【从草稿开始】按钮，即可进入空白画布。

<figure><img src="../../.gitbook/assets/image (863).png" alt=""><figcaption></figcaption></figure>

点击模块后的加号节点即可选择条件模块或动作模块，或从左侧选择希望添加的模块，完成配置后进行连线。

<figure><img src="../../.gitbook/assets/image (866).png" alt=""><figcaption></figcaption></figure>

完成配置后发布即刻生效。
