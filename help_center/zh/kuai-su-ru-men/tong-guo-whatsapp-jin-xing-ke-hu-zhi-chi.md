# 通过 WhatsApp 进行客户支持

{% hint style="info" %}
在当今数字化时代，客户期望能够随时随地通过他们最熟悉和便捷的渠道与企业进行沟通。WhatsApp，作为全球最受欢迎的即时通讯应用之一，为企业提供了一个强大的平台来提升客户支持体验。本文将详细介绍如何通过 YCloud和WhatsApp Business API（WABA）搭建高效的客户支持系统，帮助企业通过 WhatsApp 实现卓越的客户支持，提升客户体验和业务效率。
{% endhint %}

> **以下将详细介绍如何开始通过 WhatsApp 开展客户支持**

## **前置准备**

在通过 WhatsApp 进行客户支持服务之前，您需要完成以下步骤：

### **步骤一：YCloud 账户创建**

[点击注册](https://www.ycloud.com/console/#/entry/login?lastPath=https%3A%2F%2Fwww.ycloud.com%2Fconsole%2F%23%2Fapp%2Fdashboard%2FgetStarted)您的 YCloud 账户。

### **步骤二：创建 WABA 账户**

需要准备的资料：

* 一个 Facebook 账号
*   电话号码

    * 该电话号码必须能够接收语音呼叫或短信。
    * 该号码之前没有注册过 WhatsApp App 或者商业账户。

    <figure><img src="../.gitbook/assets/image (140).png" alt=""><figcaption></figcaption></figure>

详细操作参考：[创建WhatsApp Business API账户](https://helpdocs.ycloud.com/help-center/zh/kuai-su-ru-men/chuang-jian-whatsapp-business-api-zhang-hu?fallback=true)

## 通过 WhatsApp 进行客户支持

### **步骤一：邀请客服团队加入**

邀请路径：

* 左下角账户 > [Settings](https://www.ycloud.com/console/#/app/globalSettings/general/companyInfo) > [Users and teams ](https://www.ycloud.com/console/#/app/globalSettings/general/usersAndTeams)> [Invite user](https://www.ycloud.com/console/#/app/globalSettings/general/usersAndTeams)。

角色选择 Service

<figure><img src="../.gitbook/assets/image (141).png" alt=""><figcaption></figcaption></figure>

详细操作参考：[邀请用户和团队](https://helpdocs.ycloud.com/help-center/zh/zhang-hu-guan-li/yong-hu-he-tuan-dui)

### **步骤二：设置客户分配规则**

将步骤一邀请的客服，配置到WhatsApp商业号码的分配规则中，以保证他们可以及时收到来自意向客户的咨询。

<figure><img src="../.gitbook/assets/image (142).png" alt=""><figcaption></figcaption></figure>

详细操作参考：[对话分配规则](https://helpdocs.ycloud.com/help-center/zh/whatsapp-accounts-zhang-hao-guan-li/shou-ji-hao-ma-guan-li/dui-hua-fen-pei-gui-ze)

### **步骤三：配置自动化消息**

可实现自动回复未分配对话、在排队中的会话及超时回复等，提升客服沟通效率、优化客户体验。

操作路径： [WhatsApp accounts](https://www.ycloud.com/console/#/app/dashboard/account) > [号码的Settings ](https://www.ycloud.com/console/#/app/dashboard/accountSetting/profile?redirectPath=%2Fapp%2Fdashboard%2Faccount)> [Automation](https://www.ycloud.com/console/#/app/dashboard/accountSetting/automations?redirectPath=%2Fapp%2Fdashboard%2Faccount)

<figure><img src="../.gitbook/assets/image (143).png" alt=""><figcaption></figcaption></figure>

详细操作参考：[自动化消息](https://helpdocs.ycloud.com/help-center/zh/whatsapp-accounts-zhang-hao-guan-li/shou-ji-hao-ma-guan-li/zi-dong-hua#ice-breakers-po-bing-ti-shi)

### **步骤四：配置Chatbot自动响应客户咨询**

Chatbot是YCloud基于WhatsApp开发的自动化流程机器人。通过识别客户的消息内容，可以进行自动对话，或者给客户进行打标、退订等操作。企业可以创建多种不同类型的Chatbot，来帮助企业实现高效回复和降低成本。

1. [YCloud 后台](https://www.ycloud.com/console/#/app/getStarted) > [Chatbot](https://www.ycloud.com/console/#/app/chatbot/list) > [Create Chatbot](https://www.ycloud.com/console/#/app/chatbot/list) ,并设置Chatbot的基础配置

<figure><img src="../.gitbook/assets/image (144).png" alt=""><figcaption></figcaption></figure>

详细操作参考: [创建一个Chatbot](https://helpdocs.ycloud.com/help-center/zh/chatbot/chuang-jian-yi-ge-chatbot)

2. 创建 Chatbot Flow

* 设置 Flaw 的trigger

<figure><img src="../.gitbook/assets/image (145).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (146).png" alt=""><figcaption></figcaption></figure>

* 激活Flow

<figure><img src="../.gitbook/assets/image (147).png" alt=""><figcaption></figcaption></figure>

详细操作参考:[创建一个Flow](https://helpdocs.ycloud.com/help-center/zh/chatbot/chuang-jian-yi-ge-flow)

3. 号码关联Chatbot

每个号码都可配置一个机器人，它会在配置的工作时间内自动接待客户。

操作路径：[WhatsApp accounts](https://www.ycloud.com/console/#/app/dashboard/account) > [号码的Settings](https://www.ycloud.com/console/#/app/dashboard/accountSetting/profile?redirectPath=%2Fapp%2Fdashboard%2Faccount) > [Chatbot](https://www.ycloud.com/console/#/app/dashboard/accountSetting/chatbot?redirectPath=%2Fapp%2Fdashboard%2Faccount)

添加要配置的Chatbot

<figure><img src="../.gitbook/assets/image (148).png" alt=""><figcaption></figcaption></figure>

设置Chatbot的接待时间

<figure><img src="../.gitbook/assets/image (149).png" alt=""><figcaption></figcaption></figure>

详细操作参考：[Chatbot接待设置](https://helpdocs.ycloud.com/help-center/zh/whatsapp-accounts-zhang-hao-guan-li/shou-ji-hao-ma-guan-li/ji-qi-ren-jie-dai-she-zhi)

### **步骤五：培训客服上线接待**

Inbox是YCloud的重要功能，为服务团队提供高效客户沟通与管理平台。培训客服团队使用Inbox至关重要，因为这能帮助他们熟练掌握平台的各项功能，如共享收件箱、坐席分配、客户数据管理、分析报告等，从而提升工作效率，快速响应客户需求，提高客户满意度和忠诚度。&#x20;

详细操作参考：[服务团队如何使用Inbox](https://helpdocs.ycloud.com/help-center/zh/inbox/zui-jia-shi-jian/fu-wu-tuan-dui-ru-he-shi-yong-inbox)

### **步骤六：监控和绩效分析**

* [看分析](https://www.ycloud.com/console/#/app/inbox/analytics)

掌握如何通过Inbox统计报告了解团队表现至关重要，因为这能帮助管理者基于数据做出科学决策，优化资源分配，提升团队效率和绩效，及时发现并解决问题，从而推动团队和企业的发展。

<figure><img src="../.gitbook/assets/image (151).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (152).png" alt=""><figcaption></figcaption></figure>

详细操作参考：[Inbox数据分析](https://helpdocs.ycloud.com/help-center/zh/inbox/inbox-shu-ju-fen-xi)

* [查看会话日志](https://www.ycloud.com/console/#/app/inbox/conversation)

当团队主管需要对团队成员的会话进行定期巡检或抽查质检时，会话日志往往会派上很大的用场。 会话日志是会话记录的管理后台，所有发生过的会话都将被记录在其中。此外，会话日志还提供了便捷的检索功能，便于管理人员迅速定位具体对话，并通过会话详情页查看会话的具体详情。

<figure><img src="../.gitbook/assets/image (153).png" alt=""><figcaption></figcaption></figure>

详细操作参考：[会话日志](https://helpdocs.ycloud.com/help-center/zh/inbox/hui-hua-ri-zhi)

## 最佳实践

### **设计聊天接入点**

设计WhatsApp聊天接入点，旨在提升客户体验，让用户更便捷地与企业沟通，减少等待和操作步骤，从而提高客户满意度。同时，这有助于提高转化率，因方便的沟通渠道能增加用户互动和购买意愿。此外，多渠道接入点还能增强品牌曝光，吸引更多潜在客户，并优化客户服务，使客服人员能全面了解客户背景，提供个性化服务。总之，这些设计能让企业充分借助WhatsApp的即时通讯优势，提升客户体验和业务效率。

### **为什么要设计WhatsApp聊天接入点**

{% hint style="success" %}
* **提升客户体验**：通过提供多种接入点，用户可以更方便地与企业沟通，减少等待时间和操作步骤，提高客户满意度。
* **提高转化率**：方便的沟通渠道能够增加用户与企业的互动，提高用户的购买意愿和转化率。
* **增强品牌曝光**：在多个渠道提供WhatsApp接入点，可以增加品牌的曝光度，吸引更多潜在客户。
* **优化客户服务**：整合多个渠道的客户沟通记录，客服人员可以更全面地了解客户背景，提供更个性化的服务。
{% endhint %}

通过这些设计，企业可以更好地利用WhatsApp的即时通讯功能，提升客户体验和业务效率。

<figure><img src="../.gitbook/assets/image (154).png" alt=""><figcaption></figcaption></figure>

### **聊天接入点的常见渠道途径：**

为了满足客户在不同场景下寻求帮助的需求，我们可以在相应位置配置WhatsApp客户聊天接入点，引导客户通过WhatsApp进行咨询。

1. **APP-link**

通过在应用程序中嵌入WhatsApp链接，用户可以一键打开WhatsApp与企业进行沟通。例如，可以在电商应用的商品详情页添加“点击联系客服”按钮，用户点击后直接跳转到WhatsApp聊天界面。

2. **门店台卡**

在实体门店的显眼位置放置带有WhatsApp二维码或链接的台卡，顾客扫描二维码或点击链接即可与企业客服进行即时沟通，方便顾客咨询产品信息或售后服务。

3. **网站上小部件**

在企业网站上添加WhatsApp聊天小部件，用户在浏览网站时可以方便地发起对话。这可以通过在网站的侧边栏、底部或特定页面添加WhatsApp按钮实现。例如，用户在查看产品详情时，点击WhatsApp按钮即可直接与客服人员沟通，获取更多产品信息或解决疑问。

4. **社交媒体平台**

在企业的社交媒体账号（如Facebook、Instagram等）上添加WhatsApp聊天按钮或链接，用户在浏览社交媒体内容时可以方便地与企业进行互动，提升用户参与度和客户体验。

5. **业务工具集成**

将WhatsApp集成到企业的业务工具中，如CRM系统、帮助台平台等。这样，客服团队可以在熟悉的工具中管理WhatsApp聊天，提高工作效率和客户服务质量。这些渠道途径可以帮助企业更有效地与客户进行沟通，提升客户体验和业务效率。

详细操作参考：[生成号码的分享链接、二维码或网页聊天插件](https://helpdocs.ycloud.com/help-center/zh/whatsapp-accounts-zhang-hao-guan-li/shou-ji-hao-ma-guan-li/liao-tian-lian-jie)

{% hint style="info" %}
通过本文的介绍，您已经了解了如何通过 YCloud 平台和 WhatsApp 进行客户支持的全过程。从账户创建到配置自动化消息，再到培训客服团队和监控绩效，每一步都旨在提升客户体验和业务效率。设计聊天接入点是实现这一目标的关键，它不仅方便客户与企业沟通，还能增强品牌曝光度和客户转化率。希望本文能帮助您的企业更好地利 WhatsApp这一强大的工具，提升客户支持水平，增强市场竞争力，赢得客户的信任和忠诚。如果您有任何疑问或需要进一步的帮助，请随时联系YCloud团队，我们期待与您携手共创美好未来。
{% endhint %}
