---
description: 本篇讲述WhatsApp复制验证码模板，即Copy Code Authentication Templates
---

# 复制验证码身份验证模板

复制代码身份验证模板允许您向用户发送一次性密码或代码以及复制代码按钮。当 WhatsApp 用户点击复制代码按钮时，WhatsApp 客户端会将密码或代码复制到设备的剪贴板。然后，用户可以切换到您的应用并将密码或代码粘贴到您的应用中。

<figure><img src="../../../.gitbook/assets/image (662).png" alt="" width="563"><figcaption></figcaption></figure>

复制代码按钮身份验证模板包括：

* 预设文本： _\<VERIFICATION\_CODE>是您的验证码。_
* 可选的安全免责声明：_为了您的安全，请不要共享此代码。_
* 可选的过期警告（可选）：_此代码将在 \<NUM\_MINUTES> 分钟后过期。_
* 复制代码按钮。
* 消息有效期：如果消息没有在有效期范围内送达，您将不会被收取费用，您的客户将不会看到该消息。

#### 限制 <a href="#limitations" id="limitations"></a>

不支持 URL、媒体和表情符号。



## **模板创建**

### **通过API创建示例请求（复制代码）**

{% embed url="https://docs.ycloud.com/reference/whatsapp-template-creation-examples#authentication-template-with-copy-code-button" %}

### 使用[YCloud 后台](https://www.ycloud.com/console/#/app/whatsApp/template)手动创建

{% content-ref url="../../../whatsapp-accounts-zhang-hao-guan-li/mu-ban-guan-li/chuang-jian-mu-ban/" %}
[chuang-jian-mu-ban](../../../whatsapp-accounts-zhang-hao-guan-li/mu-ban-guan-li/chuang-jian-mu-ban/)
{% endcontent-ref %}

##

## **发送身份验证模板消息**

使用YCloud [whatsapp api](https://docs.ycloud.com/reference/whatsapp_message-send-directly)发送身份验证模板消息。

<br>
