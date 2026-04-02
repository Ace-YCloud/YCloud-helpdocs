---
description: 本文档介绍了限时优惠模板及其使用方法。
---

# 限时优惠模板

{% hint style="info" %}
限时优惠模板仅支持创建，可通过API发送
{% endhint %}

限时优惠模板可让您在模板消息中显示优惠代码的到期日期和正在运行的倒计时器，让您轻松传达限时优惠并推动客户参与。限时优惠模版仅适用于营销模版消息。

<figure><img src="../../.gitbook/assets/image (550).png" alt="" width="363"><figcaption></figcaption></figure>

### 限时优惠组件 <a href="#limitations" id="limitations"></a>

限时优惠模版由标题、限时优惠组件、正文和按钮组成。限时优惠组件包含限时优惠标题、限时优惠时间和限时优惠码，规则如下：

* 标题为必填。
* 限时按钮默认为开，您可以手动关闭。若限时按钮打开，您可以在发送这个模版的时候上传限时优惠的具体时间。⚠️ 创建限时优惠模版的时候不需要上传具体限时优惠时间。
* 若您选择添加复制优惠码按钮，并且填写了示例优惠码，则会显示限时优惠码。否则，不显示限时优惠码。
* 访问网站按钮为必填，复制优惠码为选填。

### 创建限时优惠模版

您可以在YCloud的模版里创建限时优惠模版。

首先，在在营销模版目录下选择限时优惠模版。

<figure><img src="../../.gitbook/assets/image (870).png" alt=""><figcaption></figcaption></figure>

然后，依次填充标题、限时优惠组件、正文和按钮。

<figure><img src="../../.gitbook/assets/image (872).png" alt=""><figcaption></figcaption></figure>

⚠️ 使用 WhatsApp 网页应用程序或桌面应用程序查看限时优惠模板消息的用户将看不到该优惠，但会看到一条消息，表明他们已收到一条消息。

💡您可以通过调用API的方式发送轮播模版。

