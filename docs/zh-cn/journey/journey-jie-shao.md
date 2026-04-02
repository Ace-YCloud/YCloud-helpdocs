---
doc_id: doc_journey_journey_jie_shao
language: zh-CN
title: "Journey介绍"
slug: journey-jie-shao
path: journey/journey-jie-shao
document_group: journey
path_in_group: journey-jie-shao
parent_id: doc_journey
order: 540
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T11:17:05.492Z
updated_at: 2026-04-02T11:17:05.492Z
last_synced_at: 2026-04-02T11:17:05.492Z
tags:
---

# Journey介绍

Journey 是帮助企业基于客户行为触发一系列动作的自动化流程。您可以使用它对触发了事件的客户进行消息发送，自动打标签等。

举例：

电商场景下，您可以基于客户的生命周期进行消息通知，如：订阅成功通知、购物车弃购通知、订单催付、发货提醒、订单取消提醒等。

App的企业，可以使用Journey进行客户的激活。例如当客户注册App后，等待N天，若客户还未进行激活，可以自动给客户发送一条促激活的消息。



## 了解Journey的功能：

### Journey包含的组件：

<table><thead><tr><th width="118">组件</th><th width="304">功能</th><th></th></tr></thead><tbody><tr><td>Trigger</td><td><p>Trigger是Journey的核心功能，是用于设置触发的事件和条件。</p><p>满足Trigger中所有条件的用户才会触发Journey</p><p></p></td><td><img src="../.gitbook/assets/image (592).png" alt="" data-size="original"></td></tr><tr><td>Send template</td><td>发送模板组件，设置要发送的内容</td><td><img src="../.gitbook/assets/image (593).png" alt="" data-size="original"></td></tr><tr><td>Message status rule</td><td>判断模板消息的状态</td><td><img src="../.gitbook/assets/image (594).png" alt="" data-size="original"></td></tr><tr><td>Add tag</td><td>打标签</td><td><img src="../.gitbook/assets/image (595).png" alt="" data-size="original"></td></tr><tr><td>Wait</td><td>等待</td><td><img src="../.gitbook/assets/image (596).png" alt="" data-size="original"></td></tr></tbody></table>

### 组件连接

组件和组件之间需要进行连接，根据连接后的顺序进行执行。

<figure><img src="../.gitbook/assets/image (597).png" alt=""><figcaption></figcaption></figure>

### 设置Journey的目标和退出条件

#### **目标**：

用于统计Journey的效果。通过设置目标，在Journey触发后持续统计客户是否满足目标条件，当客户满足后即Journey的目标完成数量+1。

{% hint style="info" %}
注意：目标仅用于数据统计，完成目标并不表示客户会退出Journey。只有满足[**退出条件**](journey-jie-shao.md#tui-chu-tiao-jian)，或者执行完Journey最后一个组件后才会退出。
{% endhint %}

#### **退出条件**：

当用户进入Journey后，会持续判断用户是否符合了退出条件，符合后无论用户在Journey的哪个阶段，都会立即退出，即不再执行后面的组件。

<figure><img src="../.gitbook/assets/image (599).png" alt=""><figcaption></figcaption></figure>
