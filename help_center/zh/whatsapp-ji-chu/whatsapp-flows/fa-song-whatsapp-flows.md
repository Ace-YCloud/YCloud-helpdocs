# 发送WhatsApp Flows

YCloud提供了多种发送WhatsApp Flows的方式，本文将分别介绍使用不同的YCloud产品来发送WhatsApp Flows的教程。

## 使用Campaign/API发送WhatsApp Flows

### 步骤1:

在YCloud后台创建一个带有WhatsApp Flows的消息模版。注意，只有营销/通知类型的模版支持插入WhatsApp Flows。

登陆您的YCloud账号 > Templates > 选择好对应的模版类型并编辑好内容后， 点击 Buttons > Call to action > WhatsApp Flow > 选择想要插入的WhatsApp Flow > 编辑按钮中展示的文字  > 点击 "Submit" 提交模版申请。

<figure><img src="../../.gitbook/assets/image (67).png" alt=""><figcaption></figcaption></figure>

### 步骤2: <a href="#bu-zhou-2" id="bu-zhou-2"></a>

发送WhatsApp Flows。YCloud支持使用[Campaign](https://helpdocs.ycloud.com/help-center/v/zh/campaign/chuang-jian-whatsapp-ying-xiao-huo-dong)或者[API](https://docs.ycloud.com/reference/whatsapp_message-send)来发送WhatsApp Flows。

## 使用Chatbot发送WhatsApp Flows <a href="#shi-yong-chatbot-fa-song-whatsapp-flows" id="shi-yong-chatbot-fa-song-whatsapp-flows"></a>

{% hint style="info" %}
使用Chatbot来发送WhatsApp flows。将Chatbot与WhatsApp flows结合使用，可以满足很多的场景需求，比如：订单确认与追踪，预约日程和管理，推销产品，收集用户反馈等等。
{% endhint %}

登陆您的YCloud账号 > 进入创建Chatbot flow的页面 > 点击添加Ask a question组件 > 选择WhatsApp Flow > 编辑好内容和按钮展示文字后，选择对应的WABA和您在您的bm后台中已经创建好了的WhatsApp Flows。

编辑好Chatbot flow，保存并激活后，当用户触发这个Chatbot flow，Chatbot会自动给用户发送带有WhatsApp Flow消息。

请注意：如果终端用户在chatbot发送WhatsApp Flow消息后没有进行选择和填写，chatbot将不会进行到下一个步骤，会终止在WhatsApp Flow消息这里。

<figure><img src="../../.gitbook/assets/image (68).png" alt=""><figcaption></figcaption></figure>

