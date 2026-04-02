# 外呼指南

## 要求

使用外呼WhatsApp Calling，您的商业账号必须满足以下条件：

1. BM 的message limit 到达2000.
2. 商业号码的归属国家不属于以下地区：
   1. 美国（USA)
   2. 加拿大（Canada）
   3. 土耳其（Turkey）
   4. 埃及（Egypt）
   5. 越南（Vietnam）
   6. 尼日利亚（Nigeria）

<br>

## 规则

1. 在外呼前，您的商业号必须已获取到客户的授权。
2. 72小时之内，您至多只能发送2条请求语音通话的请求消息。
3. 24小时之内，您至多可以跟客户发起5通外呼语音电话。

<br>

## 获得授权

您可以通过发送Calling request的模板，请求获取客户的授权。消息示例：<br>

<figure><img src="../.gitbook/assets/image (881).png" alt=""><figcaption></figcaption></figure>

<figure><img src="https://ycloudteam.feishu.cn/space/api/box/stream/download/asynccode/?code=NjEyY2FkMjc1MGRjMGU0Nzg2NzgzOGQ0ODU1MzgzMjlfeWtjRGVoaFVCREt2WW5aMGtFVXkweGtqM0h2dEMwbERfVG9rZW46STdVcWJOM2phb2xsVkl4Y0g3VWNYQ3ZNblhlXzE3NjM5ODI5MzM6MTc2Mzk4NjUzM19WNA" alt=""><figcaption></figcaption></figure>

### 详细步骤

#### 1. 创建Calling request 模板

入口: Templates> Caling request

<figure><img src="../.gitbook/assets/image (882).png" alt=""><figcaption></figcaption></figure>

<figure><img src="https://ycloudteam.feishu.cn/space/api/box/stream/download/asynccode/?code=NWMwNTY0N2JlYjhlYzE2OTBiYmQ4NjA2YWNiNTIxNDlfZzhiaU9FeFJjOTNuaW80UU9BTjYzN2hVSUNhVEZIemJfVG9rZW46VFBid2JDOXpOb1lrNTB4Y1loNWNUaGFJbnhiXzE3NjM5ODI5MzM6MTc2Mzk4NjUzM19WNA" alt=""><figcaption></figcaption></figure>

输入模板内容

<figure><img src="../.gitbook/assets/image (883).png" alt=""><figcaption></figcaption></figure>

<figure><img src="https://ycloudteam.feishu.cn/space/api/box/stream/download/asynccode/?code=Zjk0ZDNkZTU0NzRmNDA3NDVkMmY1MGJiYjhiZTdiZTdfSlJiT29XWXdMYWxHQjdBdFZ1QnZ6dXREUTM4TjN3bFdfVG9rZW46TldsTWIwUnZLb0t1OXN4bHVneGNIMFVybkNkXzE3NjM5ODI5MzM6MTc2Mzk4NjUzM19WNA" alt=""><figcaption></figcaption></figure>

#### 2. 发送Calling request 模板

当您的Calling request 模板审核通过，您可以使用Inbox 或者Campaign 给客户发送语音通过的请求

**Inbox**

如果您有单个客户需要进行通话，可点击Inbox以下两个按钮分别给新客户和已聊天的客户发送 Calling request模板消息。<br>

<figure><img src="../.gitbook/assets/image (884).png" alt=""><figcaption></figcaption></figure>

<figure><img src="https://ycloudteam.feishu.cn/space/api/box/stream/download/asynccode/?code=YTA4NDI3ZGRkMzA1OWI3MTJjNjM4MTJjZDlhNzU1YzVfVUdvOWpVTVhMTW84dGJuUW1rallHMlR5UlM4U1JyVEhfVG9rZW46SGJqaWJUSlJob3NFMmx4WHNjeGNmMWdDbk9iXzE3NjM5ODI5MzM6MTc2Mzk4NjUzM19WNA" alt=""><figcaption></figcaption></figure>

选择一个calling request模板

<figure><img src="../.gitbook/assets/image (885).png" alt=""><figcaption></figcaption></figure>





**Campaign**

如果你有大批量的请求，可以使用Campaign进行下发，选择Calling request的模板即可。

<figure><img src="../.gitbook/assets/image (886).png" alt=""><figcaption></figcaption></figure>

<figure><img src="https://ycloudteam.feishu.cn/space/api/box/stream/download/asynccode/?code=OGQ3N2RjYWJlYWI4YTQ3NTVhZTlmMDc5NzI3MzBjM2Rfcmo2bEFsWE44UlNJQlE2NXpwVXZKQk9scGVUWjhrUnZfVG9rZW46TEZTRWJnb3Zlb1FVSHV4WUpBUWN3Z2g3blZjXzE3NjM5ODI5MzM6MTc2Mzk4NjUzM19WNA" alt=""><figcaption></figcaption></figure>

\
发送完成后可以在Campaign的统计中查看到客户的授权情况。

<figure><img src="../.gitbook/assets/image (887).png" alt=""><figcaption></figcaption></figure>

<figure><img src="https://ycloudteam.feishu.cn/space/api/box/stream/download/asynccode/?code=Y2M1N2JiZTliYzJlMTM4ODk0NDZhNjhjYjc3ZWJjZTZfSWp0clNjZUZxTlRMV2dWT2ZXME9iTHVTc0Z6OTVPRVRfVG9rZW46TlJ3MWJVMkhhb0JSeVJ4Mk5MZmMxbnlnbkpjXzE3NjM5ODI5MzM6MTc2Mzk4NjUzM19WNA" alt=""><figcaption></figcaption></figure>

## 查看授权客户

当用户完成授权后，您可以在Calling 平台的Permission list中查看。

{% hint style="warning" %}
该页面含权限控制，您只能看到自己权限范围内的客户名单。
{% endhint %}

<figure><img src="https://ycloudteam.feishu.cn/space/api/box/stream/download/asynccode/?code=ODlhMmZjYTgyMDRhYzRmOGQ1MjFhOTQ0ZjI5MjJhZjRfMTFxdHpSTHR4MEp6TDFxb0tVTGF3ODFmWTk3NTd3dkpfVG9rZW46QkVwOGJ2SVNPb0w5RHB4NDNUR2NYQ252blJnXzE3NjM5ODI5MzM6MTc2Mzk4NjUzM19WNA" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (888).png" alt=""><figcaption></figcaption></figure>

## 发起外呼

1. **您可以在 Permission list中点击Call 按钮直接对已经授权的客户发起语音电话。**

客户的授权是有有效性的，企业仅可在有效时间内对他进行外呼。在呼叫前，请确保自己有使用该商业号码进行外呼的权限。配置参考 :  [#pei-zhi-wai-hu-quan-xian](overview.md#pei-zhi-wai-hu-quan-xian "mention")<br>

<figure><img src="../.gitbook/assets/image (889).png" alt=""><figcaption></figcaption></figure>

<figure><img src="https://ycloudteam.feishu.cn/space/api/box/stream/download/asynccode/?code=NDhkYzQyMTAwNmEyMWQ0Y2Q2NTViOWU1NWZhY2ViZjhfU3ZGR3lrZ2V4S3Vtd3lLWlNmUnc1eDBRdmZYeXlPbmhfVG9rZW46RmV6QWJUWUQwb3pWMmN4TWlud2NCVVdnbmNiXzE3NjM5ODI5MzM6MTc2Mzk4NjUzM19WNA" alt=""><figcaption></figcaption></figure>



2. **在Calling页面中直接发起外呼**

点击Calling 页面中的\[+ Calling]输入用户的手机号码并选择您要使用的商业号码进行外呼。

{% hint style="warning" %}
在呼叫前，请确保：

1. 自己有使用该商业号码进行外呼的权限。
2. 该用户已经接受了您的外呼请求。
{% endhint %}

<figure><img src="../.gitbook/assets/image (890).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (891).png" alt=""><figcaption></figcaption></figure>



3. **在Inbox中发起外呼**

[**详细步骤参考**](https://helpdocs.ycloud.com/help-center/zh/inbox/inbox-calling#er-zhu-dong-fa-qi-wai-hu)

<figure><img src="../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>
