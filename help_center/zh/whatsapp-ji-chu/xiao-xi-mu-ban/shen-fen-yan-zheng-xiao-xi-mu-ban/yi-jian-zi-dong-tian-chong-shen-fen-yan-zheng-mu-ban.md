---
description: 本篇讲述
---

# 一键自动填充身份验证模板

一键自动填充身份验证模板允许您向用户发送验证码以及一键自动填充按钮。当 WhatsApp 用户点击自动填充按钮时，WhatsApp 客户端会触发一项活动，打开您的应用并向其发送密码或代码。

<figure><img src="../../../.gitbook/assets/image (663).png" alt="" width="563"><figcaption></figcaption></figure>

一键自动填充按钮身份验证模板包括：

* 预设文本： _\<VERIFICATION\_CODE>是您的验证码。_
* 可选的安全免责声明：_为了您的安全，请不要共享此代码。_
* 可选的过期警告（可选）：_此代码将在 \<NUM\_MINUTES> 分钟后过期。_
* 一键自动填充按钮。
* 消息有效期：如果消息没有在有效期范围内送达，您将不会被收取费用，您的客户将不会看到该消息。

#### 限制 <a href="#limitations" id="limitations"></a>

一键自动填充按钮仅支持 Android。如果您将身份验证模板发送给使用非 Android 设备的 WhatsApp 用户，WhatsApp 客户端将显示复制代码按钮。

不支持 URL、媒体和表情符号。



## **模板创建**

### **通过API创建示例请求（复制代码）**

{% embed url="https://docs.ycloud.com/reference/whatsapp-template-creation-examples#authentication-template-with-one-tap-button" %}

### 使用[YCloud 后台](https://www.ycloud.com/console/#/app/whatsApp/template)手动创建

{% content-ref url="../../../whatsapp-accounts-zhang-hao-guan-li/mu-ban-guan-li/chuang-jian-mu-ban/" %}
[chuang-jian-mu-ban](../../../whatsapp-accounts-zhang-hao-guan-li/mu-ban-guan-li/chuang-jian-mu-ban/)
{% endcontent-ref %}

##

## **应用程序签名密钥哈希**

如果您正在创建使用一键自动填充按钮的身份验证模板，则必须在组件数组中包含您的应用签名密钥哈希。

要计算您的哈希值，请按照 Google 的说明[计算应用的哈希字符串](https://github.com/googlearchive/android-credentials/blob/master/sms-verification/bin/sms_retriever_hash_v9.sh?fbclid=IwAR2owG2gEeRbwrEJfX7OOXMotU8-Q1I6rHWIBlyo-cD8RviX87ibyyXRkus)。

或者，如果您按照 Google 的说明下载应用签名密钥证书（步骤 1），则可以将您的证书与[sms\_retriever\_hash\_v9.sh](https://developers.google.com/identity/sms-retriever/verify?fbclid=IwAR0VUfZEdsoKH5RkJQuba7HIdPtoAFHxQZg9hpybumuMdqvzBeg6aHRI7l0#computing_your_apps_hash_string) shell 脚本一起使用来计算哈希值。例如：

```
./sms_retriever_hash_v9.sh --package "com.example.myapplication" --keystore ~/.android/debug.keystore
```

<br>

## **发送身份验证模板消息**

使用YCloud [whatsapp api](https://docs.ycloud.com/reference/whatsapp_message-send-directly)发送身份验证模板消息。

请注意，如果您要发送具有一键自动填充按钮的身份验证模板，则必须首先在您的应用和 WhatsApp Messenger 或 WhatsApp Business 之间发起握手。请参阅下面的握手。



## **握手**

如果您的任何身份验证模板使用一键自动填充按钮，则您的应用必须能够启动“握手”。

握手是您实现的 Android 意图和公共类，但我们可以从 WhatsApp 应用程序或 WhatsApp Business 应用程序开始。

当您应用中的用户请求一次性密码或验证码并选择将其发送到他们的 WhatsApp 号码时，首先进行握手，然后调用我们的 API 发送身份验证模板消息。当 WhatsApp 应用或 WhatsApp Business 应用收到该消息时，它将执行资格检查，如果没有错误，则启动意图并向用户显示该消息。最后，当用户点击消息的一键自动填充按钮时，我们会自动加载您的应用并向其传递密码或代码。

<figure><img src="https://files.readme.io/ee259fa-image.png" alt=""><figcaption></figcaption></figure>

如果您在发送消息之前没有进行握手，或者消息未通过资格检查，则传递的消息将显示复制代码按钮，而不是一键按钮。

<br>

### **资格审查**

WhatsApp 应用程序或 WhatsApp Business 应用程序在收到身份验证模板消息时会执行以下检查。如果任何检查失败，一键自动填充按钮将被替换为复制代码按钮。

* 握手发生在不超过 10 分钟前。
* 消息中的软件包名称（在模板创建时在 components 数组中的**package\_name**属性中定义）与 Intent 上设置的软件包名称相匹配。匹配是通过应用程序提供的**PendingIntent**对象中调用的**getCreatorPackage方法来确定的。请参阅**[组件](https://developers.facebook.com/docs/whatsapp/business-management-api/authentication-templates#components)和公共类。
* 消息中的应用签名密钥哈希（在模板创建时在组件数组中的 signature\_hash 属性中定义）与您安装的应用的签名密钥哈希相匹配。请参阅[组件](https://developers.facebook.com/docs/whatsapp/business-management-api/authentication-templates#components)
* 该消息包含一键自动填充按钮文本。
* 您的应用已定义活动来接收密码或代码。请参阅下面的[活动](https://developers.facebook.com/docs/whatsapp/business-management-api/authentication-templates#components)。

<br>

### **Android 通知**

仅当满足以下条件时，用户的 Android 设备上才会显示表明收到 WhatsApp 身份验证模板消息的 Android 通知：

* 用户使用接收消息的电话号码（帐户）登录 WhatsApp 应用程序或 WhatsApp Business 应用程序。
* 用户已登录您的应用程序。
* Android 操作系统为 KitKat (4.4，API 19) 或更高版本。
* 在 WhatsApp 应用程序或 WhatsApp Business 应用程序中已启用显示通知（设置 > 通知）。
* 已为 WhatsApp 应用程序或 WhatsApp Business 应用程序启用设备级别通知。
* 用户与您的企业之间在 WhatsApp 应用程序或 WhatsApp Business 应用程序中的先前消息线程不会被静音。

<br>

### **客户端实现**

在您的应用中实现以下活动和类。



### **活动**

声明一个可以接收一次性密码或代码的活动和意图过滤器。意图过滤器必须具有操作名称**com.whatsapp.otp.OTP\_RETRIEVED**。

```
<activity
   android:name=".ReceiveCodeActivity"
   android:enabled="true"
   android:exported="true"
   android:launchMode="standard">
   <intent-filter>
       <action android:name="com.whatsapp.otp.OTP_RETRIEVED" />
   </intent-filter>
</activity>
```

这是 WhatsApp 应用程序或 WhatsApp Business 应用程序在收到身份验证模板消息并通过所有资格检查后将启动的活动。

<br>

### **公开课**

定义可以在将代码传递到您的应用程序后接受该代码的活动公共类。

```
public class ReceiveCodeActivity extends AppCompatActivity {

   @Override
   protected void onCreate(Bundle savedInstanceState) {
       super.onCreate(savedInstanceState);
       Intent intent = getIntent();
       // retrieve PendingIntent from extras bundle
       PendingIntent pendingIntent = intent.getParcelableExtra("_ci_");
       // verify source of the pendingIntent
       String pendingIntentCreatorPackage = pendingIntent.getCreatorPackage();
       // check if creatorPackage is "com.whatsapp" -> WA consumer app Or
       // "com.whatsapp.w4b" -> WA business app
       if ("com.whatsapp".equals(creatorPackage) || "com.whatsapp.w4b".equals(creatorPackage)) {
         // use OTP code
         String otpCode = intent.getStringExtra("code");
       }
   }
}
```

\
<br>

### **发起握手**

此示例演示了使用 WhatsApp 应用程序或 WhatsApp Business 应用程序发起握手的一种方法。

```
public void sendOtpIntentToWhatsApp() {
   // Send OTP_REQUESTED intent to both WA and WA Business App
   sendOtpIntentToWhatsApp("com.whatsapp");
   sendOtpIntentToWhatsApp("com.whatsapp.w4b");
}

private void sendOtpIntentToWhatsApp(String packageName) {

  /**
  * Starting with Build.VERSION_CODES.S, it will be required to explicitly 
  * specify the mutability of  PendingIntents on creation with either 
  * (@link #FLAG_IMMUTABLE} or FLAG_MUTABLE
  */
  int flags = Build.VERSION.SDK_INT >= Build.VERSION_CODES.S ? FLAG_IMMUTABLE : 0;
  PendingIntent pi = PendingIntent.getActivity(
      getApplicationContext(), 
      0, 
      new Intent(), 
      flags);


  // Send OTP_REQUESTED intent to WhatsApp
  Intent intentToWhatsApp = new Intent();
  intentToWhatsApp.setPackage(packageName);
  intentToWhatsApp.setAction("com.whatsapp.otp.OTP_REQUESTED");
  // WA will use this to verify the identity of the caller app.
  Bundle extras = intentToWhatsApp.getExtras();
  if (extras == null) {
     extras = new Bundle();
  }
  extras.putParcelable("_ci_", pi);
  intentToWhatsApp.putExtras(extras);
  getApplicationContext().sendBroadcast(intentToWhatsApp);
}
```



