# 零点击身份验证模板

零点击身份验证模板允许您的用户通过 WhatsApp 接收一次性密码或代码，而无需离开您的应用程序。

当您应用中的用户请求密码或代码并且您使用零点击身份验证模板提供该密码或代码时，WhatsApp 客户端只需广播所包含的密码或代码，您的应用就可以使用广播接收器立即捕获它。

从用户的角度来看，他们在您的应用中请求密码或代码，该密码或代码会自动显示在您的应用中。如果您的应用用户恰好在 WhatsApp 客户端中查看消息，他们只会看到一条显示默认固定文本的消息：_\<code> 是您的验证码。_

与一键自动填充按钮身份验证模板一样，当 WhatsApp 客户端收到包含用户密码或代码的模板消息时，我们会执行一系列资格检查。如果消息未通过此检查，并且我们无法广播密码或代码，则该消息将显示一键自动填充按钮或复制代码按钮。因此，当您创建零点击身份验证模板时，您必须在帖子正文负载中包含一键自动填充和复制代码按钮，即使用户可能永远不会看到其中一个按钮。

<figure><img src="../../../.gitbook/assets/image (664).png" alt="" width="563"><figcaption></figcaption></figure>

#### 限制 <a href="#limitations" id="limitations"></a>

零点击仅支持 Android。如果您将零点击身份验证模板发送给使用非 Android 设备的 WhatsApp 用户，WhatsApp 客户端将显示复制代码按钮。

不支持 URL、媒体和表情符号。

## **模板创建**

### **通过API创建示例请求（复制代码）**

{% embed url="https://docs.ycloud.com/reference/whatsapp-template-creation-examples#zero-tap-authentication-template" %}

### 使用[YCloud 后台](https://www.ycloud.com/console/#/app/whatsApp/template)手动创建

{% content-ref url="../../../whatsapp-accounts-zhang-hao-guan-li/mu-ban-guan-li/chuang-jian-mu-ban/" %}
[chuang-jian-mu-ban](../../../whatsapp-accounts-zhang-hao-guan-li/mu-ban-guan-li/chuang-jian-mu-ban/)
{% endcontent-ref %}



## **发送身份验证模板消息**

使用YCloud [whatsapp api](https://docs.ycloud.com/reference/whatsapp_message-send-directly)发送身份验证模板消息。

请注意，如果您要发送具有一键自动填充按钮的身份验证模板，则必须首先在您的应用和 WhatsApp Messenger 或 WhatsApp Business 之间发起握手。请参阅下面的握手。

