---
doc_id: doc_campaign_fen_xi_ying_xiao_huo_dong_shu_ju
language: zh-CN
title: "分析营销活动数据"
slug: fen-xi-ying-xiao-huo-dong-shu-ju
path: campaign/fen-xi-ying-xiao-huo-dong-shu-ju
document_group: campaign
path_in_group: fen-xi-ying-xiao-huo-dong-shu-ju
parent_id: doc_campaign
order: 0
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T07:22:09.209Z
updated_at: 2026-04-02T07:22:09.209Z
last_synced_at: 2026-04-02T07:22:09.209Z
tags:
---

# 分析营销活动数据

{% hint style="info" %}
完成Campaign发送后, 您可后台查看消息送达情况以及回复数据情况
{% endhint %}

## 步骤1

登录[YCloud账号](https://www.ycloud.com/console/#/entry/login)，导航至Campaign > Action > Analytics

<figure><img src="../.gitbook/assets/image (659).png" alt=""><figcaption></figcaption></figure>

## 步骤2

* 点击Analytics，您可查看Campaign相关数据如：发送；等待返回；送达；失败；已读以及已回复数据；
* 点击Export可下载相关数据，支持本地分析

<figure><img src="../.gitbook/assets/image (660).png" alt=""><figcaption></figcaption></figure>



## 相关参数解释

<table><thead><tr><th>状态</th><th>解释</th><th data-hidden></th></tr></thead><tbody><tr><td>Sent</td><td>此Campaign发送的消息总数</td><td></td></tr><tr><td>Processing</td><td>消息发送后，仍然保持processing状态的消息数量。processing表示已经发送，但终端还未接收成功，可能是由于网络或者未打开app导致</td><td></td></tr><tr><td>Delivered</td><td>消息发送后，终端已成功接收</td><td></td></tr><tr><td>Failed</td><td>消息发送失败。失败原因类型较多，可点击Failed状态旁的？提示查看具体原因</td><td></td></tr><tr><td>Read</td><td>终端已读了消息</td><td></td></tr><tr><td>Replied</td><td>消息在接收成功后的24小时之内，终端回复了上行消息</td><td></td></tr></tbody></table>
