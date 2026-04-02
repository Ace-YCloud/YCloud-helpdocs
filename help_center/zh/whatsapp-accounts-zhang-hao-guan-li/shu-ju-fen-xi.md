# 数据分析

数据分析页面集成了账号中所有WABA下的号码的消息记录。

## 消息到达情况统计

点击左侧导航的Home > Analytics 进入数据分析页面。默认展示消息维度的到达情况

<figure><img src="../.gitbook/assets/image (84).png" alt=""><figcaption></figcaption></figure>

##

## 对话统计&#x20;

切换Tab至Conversation按钮，可查看对话维度的统计。

（由于Meta自2025年7月1日开始，停止了会话的计费规则，所以该页面仅统计2025年7月1日前的数据）

<figure><img src="../.gitbook/assets/image (513).png" alt=""><figcaption></figcaption></figure>

## 消息记录

点击Logs查看所有消息的发送记录。可以查看条每条消息的发送时间，接收时间，发送状态。

### 发送记录

User为客户的号码，Acount为发送消息的WhatsApp api账号。

<figure><img src="../.gitbook/assets/image (500).png" alt=""><figcaption></figcaption></figure>

### 接收记录

Direction选择Inboud message，可以查看所有收到的消息。

User为客户的号码，Acount为接收到消息WhatsApp api账号。

<figure><img src="../.gitbook/assets/image (501).png" alt=""><figcaption></figcaption></figure>

## 常见问题

<details>

<summary>为什么消息的状态是Failed？</summary>

消息发送失败有很多原因。将鼠标移动到Failed旁边的问号？上可以看到具体是失败的原因。

</details>

<details>

<summary>已读时间为什么是空的？</summary>

已读回执是一个开关，若客户在手机上将开关关闭，则不会返回已读状态。

</details>

<details>

<summary>Message中不显示具体的内容，只显示[Button][Unsupported message]等提示</summary>

由于WhatsApp消息样式非常丰富，记录页面无法很好的展示一些富媒体消息和按钮互动类消息，您可以复制客户的手机号码到Inbox中搜索他的聊天内容。

</details>
