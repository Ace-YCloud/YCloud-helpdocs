---
doc_id: doc_inbox_inbox_shu_ju_fen_xi
language: zh-CN
title: "Inbox数据分析"
slug: inbox-shu-ju-fen-xi
path: inbox/inbox-shu-ju-fen-xi
document_group: inbox
path_in_group: inbox-shu-ju-fen-xi
parent_id: doc_inbox
order: 350
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T11:14:20.803Z
updated_at: 2026-04-02T11:14:20.803Z
last_synced_at: 2026-04-02T11:14:20.803Z
tags:
---

# Inbox数据分析

## 数据分析入口

入口位于Inbox左侧底部> [Analytics](https://www.ycloud.com/console/#/app/inbox/analytics)

<figure><img src="../.gitbook/assets/image (478).png" alt=""><figcaption></figcaption></figure>



## 实时概览

Inbox 实时概览为您提供实时信息（每1h更新一次）。通过这一功能，您能够清晰地了解到今日会话数，知晓当天与用户交流的总体规模；掌握客服实时接待情况。统计时区为东八区，0:00开始。默认统计所有WhatsApp账号下的情况，可通过顶部筛选单独查看指定WhatsApp号码对应Inbox的数据。

* **今日会话数：**&#x4ECA;日每小时进入的会话数

<figure><img src="../.gitbook/assets/image (75).png" alt=""><figcaption></figcaption></figure>

* **打开的会话数：**&#x5305;括开启的会话，未分配的会话，以及已被分配但还未被回复的会话

<figure><img src="../.gitbook/assets/image (480).png" alt=""><figcaption></figcaption></figure>

* **客服状态：**&#x53EF;接待状态，和离开状态

<figure><img src="../.gitbook/assets/image (481).png" alt=""><figcaption></figcaption></figure>

* **客服会话处理情况：**&#x4EE5;客服为维度，了解对应的开启会话和未回复会话数量。用于了解客服的表现和工作量。

<figure><img src="../.gitbook/assets/image (482).png" alt=""><figcaption></figcaption></figure>



## 客服

以客服为统计维度，入口如图 Analytics > [Agents](https://www.ycloud.com/console/#/app/inbox/analytics)

* 统计数据的筛选：选择统计时间段，默认展示近7天数据。最多可以选择近1年的数据。选择对应的客服，默认展示所有客服的总数据，点击“放大镜”搜索按钮进行数据加载。
* 统计数据的下载：点击"`Download`“按钮

<figure><img src="../.gitbook/assets/image (659).png" alt=""><figcaption></figcaption></figure>

#### 会话情况统计字段

会话统计单位：天：d，小时：h，分钟：m

<table><thead><tr><th width="372">字段</th><th>描述</th></tr></thead><tbody><tr><td>Conversations (Total）（会话数）</td><td>客服接待的会话数量。根据会话的创建时间统计所属的时间段。</td></tr><tr><td>Online time (Total)（在线时长）</td><td>客服在线的时间长度统计。</td></tr><tr><td>First Response Time(Avg) （平均首次响应时间）</td><td><p>进入到Inbox后会话实际的开启时间 距离 客服首次回复的时间长度的平均值。</p><p>PS：</p><ol><li>当前客服平均响应时间= 当前客服的所有首次响应时间/当前客服所有首次响应了的会话）</li><li>首次回应是哪个客服，就算是哪个客服的回应会话。</li></ol></td></tr><tr><td>Resolution Time (Avg)（会话解决时间）</td><td>进入到Inbox后会话实际的开启时间 至 会话关闭的时间</td></tr><tr><td>CSAT（用户满意度调查）</td><td>当对话结束后，用户打了4-5🌟的好评的百分比</td></tr></tbody></table>

#### 客服排行统计

排序规则：接待会话数越多的排在最前面。

<figure><img src="../.gitbook/assets/image (484).png" alt=""><figcaption></figcaption></figure>

## Inboxes

以Inboxes为统计维度，入口如图 Analytics > [Inboxes](https://www.ycloud.com/console/#/app/inbox/analytics)

* 统计数据的筛选：选择统计时间段，默认展示近7天数据。最多可以选择近1年的数据。选择对应的Inbox，默认展示所有Inbox的总数据，点击“放大镜”搜索按钮进行数据加载。
* 统计数据的下载：点击"`Download`“按钮

<figure><img src="../.gitbook/assets/image (77).png" alt=""><figcaption></figcaption></figure>

#### Inbox会话统计字段

<table><thead><tr><th width="372">字段</th><th>描述</th></tr></thead><tbody><tr><td>Conversations(Total) （接待会话数）</td><td><p>接待的总会话数量。</p><p>PS：当同一个会话被关闭，又被开启，算2次。</p></td></tr><tr><td>Inbound message(Total)（接收消息数）</td><td>接收的消息总数，非会话数量。</td></tr><tr><td>Outbound message(Total)（发送消息数）</td><td>发送的消息总数，非会话数量。</td></tr><tr><td>First Response Time (Average)（会话首次回复平均时间）</td><td>进入到Inbox后会话实际的开启时间 距离 客服首次回复的时间长度的平均值</td></tr><tr><td>Resolution Time (Average)（会话解决时间平均时间）</td><td>进入到Inbox后会话实际的开启时间 至 会话关闭的时间</td></tr></tbody></table>



## 团队

以Inboxes为统计维度，入口如图 Analytics > [Teams](https://www.ycloud.com/console/#/app/inbox/analytics)

统计数据的筛选：选择统计时间段，默认展示近7天数据。最多可以选择近1年的数据。选择对应的Team，默认展示所有Team的总数据，点击“放大镜”搜索按钮进行数据加载。

* 统计数据的下载：点击"`Download`“按钮

<figure><img src="../.gitbook/assets/image (486).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="372">字段</th><th>描述</th></tr></thead><tbody><tr><td>Conversations(Total)（团队会话数总和）</td><td>归属于当前Team的所有agent在筛选时间段内的总数。客服接待的会话数量。根据会话的创建时间统计所属的时间段。</td></tr><tr><td>Online time (Total)（团队在线时长）</td><td>归属于当前Team的所有agent在筛选时间段内的总数。客服在线的时间长度统计。包括可接待和离开两种状态。</td></tr><tr><td>First Response Time (Avg) （团队会话平均首次响应时间）</td><td>归属于当前Team的所有agent在筛选时间段内的平均值。进入到Inbox后会话的实际的开启时刻距离 客服首次回复时刻的长度的平均值。</td></tr><tr><td>Resolution time(Avg) （团队会话平均解决时间）</td><td>归属于当前Team的所有agent在筛选时间段内的平均值。进入到Inbox后会话的实际的开启时刻至 会话关闭的时刻</td></tr><tr><td>CSAT（用户满意度调查）</td><td>当对话结束后，用户打了4-5🌟的好评的百分比</td></tr></tbody></table>

**客服排行统计**

所属Team中的客服排行统计，按照总会话数排序。



## CSAT日志

以客服为统计维度，入口如图 Analytics > [CSAT Logs](https://www.ycloud.com/console/#/app/inbox/analytics)

统计数据的筛选：选择统计时间段，默认展示近7天数据。最多可以选择近1年的数据。选择对应的客服/团队，或者是筛选想要查看的评价级别，来查看对应的CSAT日志。

* 统计数据的下载：如下图所示，点击下载图标进行下载

<figure><img src="../.gitbook/assets/image (658).png" alt=""><figcaption></figcaption></figure>
