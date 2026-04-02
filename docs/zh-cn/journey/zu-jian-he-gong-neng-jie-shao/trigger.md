---
doc_id: doc_journey_zu_jian_he_gong_neng_jie_shao_trigger
language: zh-CN
title: "Trigger"
slug: trigger
path: journey/zu-jian-he-gong-neng-jie-shao/trigger
document_group: journey
path_in_group: zu-jian-he-gong-neng-jie-shao/trigger
parent_id: doc_journey_zu_jian_he_gong_neng_jie_shao
order: 10
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

# Trigger

Trigger是这个Journey的触发器，需要满足Trigger中所有条件才会成功触发。Trigger设置项包括：

## 进入Trigger

当客户满足条件，则对该客户启动Journey流程

<table><thead><tr><th width="223">设置项</th><th width="413">功能</th><th>是否必选</th></tr></thead><tbody><tr><td>何时发送</td><td><p><strong>联系人事件</strong></p><p>一旦时间发生，旅程就被触发</p><p><a href="https://helpdocs.ycloud.com/help-center/v/zh/contact/lian-xi-ren-she-zhi/lian-xi-ren-shi-jian">如何自定义联系人事件</a></p><p></p><p><strong>联系人属性规则</strong></p><p>选择一个属性变更的条件，当用户满足这个条件时会进行触发。</p><p></p><p><strong>Shopify事件</strong></p><p>当你链接了Shopify店铺，会出现这个分类</p></td><td>是</td></tr><tr><td>发件人</td><td>选择用于给客户发送消息的WhatsApp账号。（后续发送的模板都会从这个号码的归属WABA中选择）</td><td>是</td></tr><tr><td>受众</td><td><p>设置用户条件，若未设置，则不判断受众。</p><p>若设置了条件，当事件发生时，判断客户是否满足受众中设置的条件，满足的情况下触发</p></td><td>选填</td></tr><tr><td>是否过滤退订客户</td><td>勾选后，会过滤账户内的退订列表客户。不勾选则不过滤退订客户</td><td>否</td></tr><tr><td>客户触发限制</td><td><p>选项：</p><ol><li>1个用户仅触发1次</li><li>用户只要满足了条件，每次都触发</li></ol></td><td>是</td></tr></tbody></table>



## 退出Trigger（选填）

当用户进入Journey后，会持续判断用户是否符合了退出条件，符合后无论用户在Journey的哪个阶段，都会立即退出，即不再执行后续动作。



## 目标（选填）

用于统计Journey的效果。通过设置目标，在Journey触发后持续统计客户是否满足目标条件，当客户满足后即Journey的目标完成数量+1。

{% hint style="info" %}
注意：目标仅用于数据统计，完成目标并不表示客户会退出Journey。只有满足**退出Trigger**，或者执行完Journey最后一个组件后才会退出。
{% endhint %}



<figure><img src="../../.gitbook/assets/image (78).png" alt=""><figcaption><p>设置Trigger</p></figcaption></figure>
