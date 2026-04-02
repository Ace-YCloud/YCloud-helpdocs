---
description: 本文档介绍了轮播模板及其使用方法。
---

# 轮播模板

轮播模板支持发送一条带多张轮播卡片的营销消息 ，这些卡片可在水平滚动视图中查看：

<figure><img src="../../.gitbook/assets/image (26).png" alt="" width="375"><figcaption></figcaption></figure>

当用户点击商家提供的URL链接时，用户会跳转到浏览器， 这会导致用户离开WhatsApp。若您想让用户在WhatsApp内查看更多商品信息，建议使用轮播模版展示多个商品。注意：轮播模版仅适用于营销模版消息。

### 轮播卡片

轮播模版由正文和轮播卡片组成。轮播卡片由标题、正文和按钮组成。每个组件的规则如下：

* 轮播卡片数量限制在2到10张。
* 标题类型仅支持图片或视频。
* 卡片可包含1个访问网站按钮和一个快捷回复按钮
* 一个轮播模版里的所有卡片的组件需一致。

<figure><img src="../../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

### 创建轮播模版

您可以在YCloud的模版列表中创建轮播模版。

入口：WhatsApp Manager>[templates](https://www.ycloud.com/console/#/app/dashboard/template)

在营销模版库中选择轮播模版。

<figure><img src="../../.gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>

然后，依次填充正文和卡片。

在填充卡片之前先选择卡片格式，如：标题类型、按钮类型。

⚠️  请确保您在每个卡片标题里上传的媒体类型是一致的。

<figure><img src="../../.gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure>

💡您可以通过调用API的方式发送轮播模版。
