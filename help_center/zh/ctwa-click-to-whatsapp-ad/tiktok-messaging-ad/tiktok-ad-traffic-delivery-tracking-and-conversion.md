---
description: 介绍如何tiktok投放后，如何对话和查看数据、以及设置转化规则。
---

# TikTok广告：流量承接、转化回传

完成本页配置后，您可以在 YCloud 中确认 TikTok 广告带来的 WhatsApp 会话是否已正常进入 Inbox，并按需将转化事件回传给 TikTok，用于后续广告优化。本文覆盖会话验证、转化回传配置和数据查看。

{% hint style="info" %}
在继续之前，请先完成以下环节：

* [在 YCloud 中授权 TikTok 广告账户并绑定 WhatsApp Business 号码](https://helpdocs.ycloud.com/help-center/zh/ctwa-click-to-whatsapp-ad/tiktok-messaging-ad/connect-tiktok-ad-account)
* [在 TikTok Ads Manager 中创建 TikTok 消息广告](https://helpdocs.ycloud.com/help-center/zh/ctwa-click-to-whatsapp-ad/tiktok-messaging-ad/create-tiktok-instant-messaging-ad)
{% endhint %}

### 1、在 YCloud Inbox 中 与投放的流量对话

广告开始投放后，您可以在 YCloud Inbox 中查看由 TikTok 广告带来的新会话，并确认来源信息是否已正确记录。

#### 您会看到哪些信息

当用户通过 TikTok 广告进入 WhatsApp 并发起会话后，相关对话会出现在 YCloud Inbox 中。您可以通过以下信息识别该会话来自 TikTok 广告：

* 对话列表中的联系人头像旁，会显示 TikTok 广告角标。
* 联系人发送的消息中，会显示来源信息，例如 `From TikTok Ad ID: xxx`。

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2Fb4rELwGplTqje3HJSBPP%2Finbox-fromtiktokctwa-t1.png?alt=media&#x26;token=5136a75f-c44b-4101-a814-3a85dd567f55" alt=""><figcaption></figcaption></figure>

如果这是该联系人首次通过当前 WhatsApp Business 号码发起会话，您还可以在联系人详情中看到：

* `Source = TikTok Ad`：表示该联系人来自 TikTok 广告。
* `Source ID`：表示该联系人对应的 TikTok 广告 ID。

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2FXd3eW71GURfGqwCbZuwb%2Fcontact-source%3Dtiktok-ad-t1.png?alt=media&#x26;token=87cec99c-1d47-4409-9ed2-299deb540af9" alt=""><figcaption></figcaption></figure>

### 2、配置转化回传

如果您希望 TikTok 不仅记录广告点击，还能接收 WhatsApp 会话后的关键转化事件，就需要在 YCloud 中配置转化回传规则。

#### 什么是转化回传

当用户点击广告进入 WhatsApp 后，YCloud 将会话事件或后续关键行为作为事件回传给 TikTok。这样可以帮助 TikTok 更准确地评估广告效果，并为后续投放优化提供数据支持。

#### 可以回传哪些事件

YCloud 支持回传以下两类事件：

* 会话事件：用户点击广告后，在 WhatsApp 中发起会话。
* 低漏斗事件：用户在会话后完成的关键动作，例如注册、预约、下单或支付。

{% hint style="info" %}
每个广告账户只需配置一套转化回传规则。该账户下的所有广告都会按这套规则执行事件上报。
{% endhint %}

#### 开始配置

1. 在 YCloud 中进入 `CTWA > 追踪转化事件`。
2. 点击 **+ Track New Event**。
3. 按需填写以下字段：

* `Event Name`：仅用于内部管理，不影响 TikTok 事件上报。
* `Event Type`：用于定义什么行为会触发这条上报规则。
* `TikTok Event`：用于选择需要回传给 TikTok 的低漏斗事件。该字段为单选且必填。

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2FJt4QGb2pAgqgnJN1CG2s%2Fimage.png?alt=media&#x26;token=3afdbc7e-62b3-454d-ae0f-4c7c098c1114" alt=""><figcaption></figcaption></figure>

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2FlFXVmPtsFzRNwCrAAdQX%2FMy_Photor_1773062278104.png?alt=media&#x26;token=7eb57c33-e6f1-439b-8d99-a3bd15f0bc93" alt=""><figcaption></figcaption></figure>

#### 上报开关说明

* 如果关闭“上报到 TikTok”，YCloud 仍会统计该事件，但不会将事件回传给 TikTok。
* 如果打开“上报到 TikTok”，YCloud 会在规则满足时将事件回传给 TikTok。

#### 如何选择事件类型

YCloud 提供 3 种事件触发方式，您可以根据业务场景选择。



**方式一：通过联系人标签触发**

这种方式适合转化量较低、需要人工确认转化结果的场景。

1. 在 `Event Type` 中选择 **`System Events - Tag`**。
2. 输入一个（或多个）专门用于标记转化的标签。
3. 如果您需要区分不同广告或不同转化场景，建议使用不同标签分别管理。
4. 选择要回传给 TikTok 的事件类型，并根据需要开启“上报到 TikTok”。
5. 保存规则。

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2F12hp4PTEObQ8TdzGTESU%2Fchoose-eventtype-tag-t1.png?alt=media&#x26;token=ddf66914-767f-4632-97cf-7d00ad2f6614" alt=""><figcaption></figcaption></figure>

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2Fqn7BU2hDhHkHrzxJU3bv%2Fchoose-eventtype-tag%3Avalue-t1.png?alt=media&#x26;token=d5b9934c-2280-4429-97c0-7c99cc531be2" alt=""><figcaption></figcaption></figure>

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2F0m8R5UaTjsOORLzsHjqt%2Fsaved-trackevent-tag.png-t1.png?alt=media&#x26;token=b6aefbe9-e162-41e1-bb64-14a8de5f643f" alt=""><figcaption></figcaption></figure>

当联系人最近点击过相关广告，并且后续完成了您定义的转化行为后，您可以在联系人详情中为其添加该标签。

YCloud 会将该行为识别为一次转化，并按规则决定是否回传给 TikTok。



**方式二：通过自定义事件或 API 触发**

这种方式适合已有业务系统、可以通过 API 自动发送转化事件的场景，也适合已与 YCloud 完成集成的平台。

1. 在 `Event Type` 中选择自定义事件。
2. 选择一个现有的自定义事件，作为“用户已完成转化”的标识。
3. 如果当前没有可用事件，您可以先通过 API 创建自定义事件定义。
4. 选择对应的事件标签，并保存规则。
5. 根据需要选择要回传给 TikTok 的事件类型，并开启“上报到 TikTok”。

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2FQqJ0cyB7WKgjyAWMoFLO%2Fchoose-eventtype-customapi.png?alt=media&#x26;token=fd246bda-7b40-4ec7-9d73-4a9aabfa9a17" alt=""><figcaption></figcaption></figure>

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2FuilckaCBIhO3YgfhPNxG%2Fsettings-contact-customEvents-list-t1.png?alt=media&#x26;token=96321eb1-21f3-4b2f-b693-57f9b96439ac" alt=""><figcaption></figcaption></figure>

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2FdNPb7vx39hLTwz9MPDrJ%2Fchoose-eventtype-customapi-2.png?alt=media&#x26;token=6754af91-0656-4277-995f-b470b2677fa9" alt=""><figcaption></figcaption></figure>

当客户在您的业务系统中完成转化后，您可以调用 YCloud API 将该事件发送给 YCloud。YCloud 收到事件后，会结合客户近期的广告点击信息进行归因，并按规则决定是否回传给 TikTok。

相关文档：

* [创建自定义事件](https://docs.ycloud.com/reference/custom_events-create-definition)
* [发送自定义事件](https://docs.ycloud.com/reference/custom_events-send-event)

{% hint style="info" %}
当发送事件接口返回 `200` 时，表示 YCloud 已成功接收到该事件。
{% endhint %}



**方式三：通过Whatsapp会话关键词触发**

这种方式适合希望根据客户在 WhatsApp 会话中的明确表达，识别高意向线索的场景。

1. 在 `Event Type` 中选择 `System Events - Keywords`。
2. 添加一个或多个关键词。
3. 选择要回传给 TikTok 的事件类型，并根据需要开启“上报到 TikTok”。
4. 保存规则。

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2FjGpLoTOZaJWMEOrYHOGe%2Fchooose-eventtype-keyword%3Avalue-t1.png?alt=media&#x26;token=9e088950-62d1-4091-a0fc-5f24ec1f2c46" alt=""><figcaption></figcaption></figure>

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2Fj0opP799gOUNBkGCJP9q%2Fchooose-eventtype-keyword%3Avalue1.png?alt=media&#x26;token=d493797e-9a50-49da-afc8-79743b63ee12" alt=""><figcaption></figcaption></figure>

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2FzU6ZlSBPuVTOJexLTL1Q%2Ftrackevents-list-keywords-t1.png?alt=media&#x26;token=8deec69b-8a92-40a0-a90f-da7fdd98ab78" alt=""><figcaption></figcaption></figure>

当联系人最近点击过相关广告，且其在 WhatsApp 会话中发送的消息包含您设置的任一关键词时，YCloud 会将该行为识别为一次转化，并按规则决定是否回传给 TikTok。

{% hint style="info" %}
关键词触发适合识别高意向线索，但也可能出现误判。建议只设置业务含义明确的关键词。
{% endhint %}



### 3、查看广告表现与转化数据

广告开始投放后，您可以分别在 TikTok Ads Manager 和 YCloud 中查看广告表现、会话数据和转化数据。

#### 在 TikTok Ads Manager 中查看

您可以在 Campaign 模块中查看广告、广告组或广告系列的表现数据，例如花费、曝光、点击、对话和其他分析指标。

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2FbFLJKRVbUyRDrKbhw3Wv%2Ftiktok%E5%B9%BF%E5%91%8A%E5%90%8E%E5%8F%B0-%E5%B9%BF%E5%91%8A%E5%88%97%E8%A1%A8-t1.png?alt=media&#x26;token=0b9d23e9-2926-4417-936b-dbbf8ee32605" alt=""><figcaption></figcaption></figure>

您还可以在 TikTok 的事件数据页面中查看由 YCloud 回传的事件数据。

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2F2ruEDPTsjp82RIQEDIao%2Ftiktok%E5%B9%BF%E5%91%8A%E5%90%8E%E5%8F%B0-eventmanager-datasource-%E6%95%B0%E6%8D%AE%E9%9B%86%E5%88%97%E8%A1%A8-t1.png?alt=media&#x26;token=0e31e421-b163-4a6e-898a-6744439028c0" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
在数据源列表中，部分事件集名称会显示为 `WhatsApp + [Phone Number]`。您可以通过搜索 WhatsApp Business 号码，定位到对应的数据源。
{% endhint %}

点击某个消息事件集后，您可以查看该数据源下由 YCloud 上报的历史事件和相关数据。

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2FCvvRowC3jkusHPvnb3Ct%2Ftiktok%E5%90%8E%E5%8F%B0-eventmanager-%E6%95%B0%E6%8D%AE%E9%9B%86%E8%AF%A6%E6%83%85-t1.png?alt=media&#x26;token=24717e9a-1ead-4f6d-864b-330bd0924ba3" alt=""><figcaption></figcaption></figure>

其中：

* 会话事件（Conversation）由 YCloud 默认上报。
* 除会话事件外，其他事件需要您先在第七步中配置规则，并开启“上报到 TikTok”，才会显示在这里。

#### 在 YCloud 中查看

您可以在 `CTWA > Ad Manage` 中查看指定 TikTok 广告账户的广告表现和转化数据。

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2Fx4GDtQvKWBTRaMhoaCTR%2Fctwa-ad_manage-tiktokad-t1.png?alt=media&#x26;token=17d01606-9a36-490b-8673-758659abc977" alt=""><figcaption></figcaption></figure>

如果您需要查看更详细的事件明细或线索数据，可以进入 `Track Events / View Leads`。

如需查看更完整的数据说明，请参阅：[CTWA分析](https://helpdocs.ycloud.com/help-center/zh/ctwa-click-to-whatsapp-ad/ctwa-fen-xi)

### 常见问题

<details>

<summary><strong>Q：关闭“上报到 TikTok”后，YCloud 还会记录数据吗？</strong></summary>

会。YCloud 仍会统计该事件，但不会将该事件回传给 TikTok。

</details>

<details>

<summary><strong>Q：为什么我在 TikTok 中只看到会话事件，没有看到其他转化事件？</strong></summary>

除会话事件外，其他事件都需要先在第七步中配置对应规则，并开启“上报到 TikTok”，YCloud 才会将这些事件回传到 TikTok。

</details>



