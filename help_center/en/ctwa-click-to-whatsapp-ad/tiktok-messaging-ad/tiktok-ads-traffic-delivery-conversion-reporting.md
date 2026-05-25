---
description: >-
  Learn how to handle adAfter completing the setup on this page, you can confirm
  in YCloud whether WhatsApp conversations driven by TikTok traffic in YCloud
  and properly set up ad conversion & tracking.
---

# TikTok Ads: Traffic Delivery, Conversion Reporting

{% hint style="info" %}
Before continuing, make sure you have completed the following prerequisites:

* [Authorize your TikTok ad account in YCloud and bind a WhatsApp Business Number](https://helpdocs.ycloud.com/help-center/ctwa-click-to-whatsapp-ad/tiktok-messaging-ad/connect-tiktok-ad-account)
* [Create a TikTok Messaging Ad in TikTok Ads Manager](https://helpdocs.ycloud.com/help-center/ctwa-click-to-whatsapp-ad/tiktok-messaging-ad/create-tiktok-instant-messaging-ad)
{% endhint %}

### 1、 Verify That Ad Conversations Are Entering YCloud Inbox Correctly

After your ads start running, you can view new conversations driven by TikTok ads in YCloud Inbox and confirm that the source information is recorded correctly.

#### What You Will See

When a user enters WhatsApp through a TikTok ad and starts a conversation, the conversation will appear in YCloud Inbox. You can identify it as coming from a TikTok ad through the following information:

* A TikTok ad badge appears next to the contact avatar in the conversation list.
* The contact message shows source information, for example, `From TikTok Ad ID: xxx`.

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2Fb4rELwGplTqje3HJSBPP%2Finbox-fromtiktokctwa-t1.png?alt=media&#x26;token=5136a75f-c44b-4101-a814-3a85dd567f55" alt=""><figcaption></figcaption></figure>

If this is the first time the contact has started a conversation through the current WhatsApp Business Number, you can also see the following in the contact details:

* `Source = TikTok Ad`: indicates that the contact came from a TikTok ad.
* `Source ID`: indicates the TikTok ad ID associated with this contact.

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2FXd3eW71GURfGqwCbZuwb%2Fcontact-source%3Dtiktok-ad-t1.png?alt=media&#x26;token=87cec99c-1d47-4409-9ed2-299deb540af9" alt=""><figcaption></figcaption></figure>

### 2、 Set Up Conversion Reporting

If you want TikTok to receive not only ad clicks but also key conversion events after a WhatsApp conversation starts, you need to configure conversion reporting rules in YCloud.

#### What Is Conversion Reporting

Conversion reporting means that after a user clicks an ad and enters WhatsApp, YCloud sends the conversation event or a later key action back to TikTok as an event. This helps TikTok evaluate ad performance more accurately and provides data for further optimization.

#### What Events Can Be Sent Back

YCloud supports reporting the following two types of events:

* Conversation event: the user clicks the ad and starts a conversation in WhatsApp.
* Lower-funnel event: the user completes a key action after the conversation, such as registration, booking, placing an order, or making a payment.

{% hint style="info" %}
Each ad account only needs one set of conversion reporting rules. All ads under that account will follow the same reporting rules.
{% endhint %}

#### Start the Setup

1. In YCloud, go to `CTWA > Track Conversion Events`.
2. Click **+ Track New Event**.
3. Fill in the following fields as needed:

* `Event Name`: for internal management only; does not affect TikTok event reporting.
* `Event Type`: defines what action triggers this reporting rule.
* `TikTok Event`: selects which lower-funnel event should be sent back to TikTok. This field is required and supports single selection only.

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2FJt4QGb2pAgqgnJN1CG2s%2Fimage.png?alt=media&#x26;token=3afdbc7e-62b3-454d-ae0f-4c7c098c1114" alt=""><figcaption></figcaption></figure>

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2FlFXVmPtsFzRNwCrAAdQX%2FMy_Photor_1773062278104.png?alt=media&#x26;token=7eb57c33-e6f1-439b-8d99-a3bd15f0bc93" alt=""><figcaption></figcaption></figure>

#### Send-to-TikTok Toggle

* If `Send to TikTok` is turned off, YCloud will still record the event, but it will not send the event back to TikTok.
* If `Send to TikTok` is turned on, YCloud will send the event back to TikTok when the rule is triggered.

#### How to Choose an Event Type

YCloud provides 3 event trigger methods. You can choose the one that best fits your business scenario.



**Option 1: Trigger by Contact Tag**

This option is suitable for scenarios with a relatively low number of conversions and where conversion results need to be confirmed manually.

1. In `Event Type`, select `System Events - Tag`.
2. Enter a tag dedicated to marking conversions.
3. If you need to distinguish between different ads or different conversion scenarios, use different tags for separate management.
4. Select the TikTok event you want to report, and turn on `Send to TikTok` if needed.
5. Save the rule.

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2F12hp4PTEObQ8TdzGTESU%2Fchoose-eventtype-tag-t1.png?alt=media&#x26;token=ddf66914-767f-4632-97cf-7d00ad2f6614" alt=""><figcaption></figcaption></figure>

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2Fqn7BU2hDhHkHrzxJU3bv%2Fchoose-eventtype-tag%3Avalue-t1.png?alt=media&#x26;token=d5b9934c-2280-4429-97c0-7c99cc531be2" alt=""><figcaption></figcaption></figure>

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2F0m8R5UaTjsOORLzsHjqt%2Fsaved-trackevent-tag.png-t1.png?alt=media&#x26;token=b6aefbe9-e162-41e1-bb64-14a8de5f643f" alt=""><figcaption></figcaption></figure>

When a contact has recently clicked a relevant ad and later completes the conversion action you defined, you can add this tag in the contact details. YCloud will recognize this action as a conversion and decide whether to send it back to TikTok based on your rule.



**Option 2: Trigger by Custom Event or API**

This option is suitable for businesses with their own systems that can automatically send conversion events through the API, or for platforms already integrated with YCloud.

1. In `Event Type`, select a custom event.
2. Choose an existing custom event as the marker for "user has converted".
3. If there is no suitable event yet, you can first create a custom event definition through the API.
4. Select the corresponding event label and save the rule.
5. Select the TikTok event to report, and turn on `Send to TikTok` if needed.

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2FQqJ0cyB7WKgjyAWMoFLO%2Fchoose-eventtype-customapi.png?alt=media&#x26;token=fd246bda-7b40-4ec7-9d73-4a9aabfa9a17" alt=""><figcaption></figcaption></figure>

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2FuilckaCBIhO3YgfhPNxG%2Fsettings-contact-customEvents-list-t1.png?alt=media&#x26;token=96321eb1-21f3-4b2f-b693-57f9b96439ac" alt=""><figcaption></figcaption></figure>

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2FdNPb7vx39hLTwz9MPDrJ%2Fchoose-eventtype-customapi-2.png?alt=media&#x26;token=6754af91-0656-4277-995f-b470b2677fa9" alt=""><figcaption></figcaption></figure>

When a customer converts in your business system, you can call the YCloud API to send the event to YCloud. After receiving the event, YCloud will perform attribution based on the customer's recent ad-click data and decide whether to send it back to TikTok according to your rule.

Related documentation:

* [Create a custom event](https://docs.ycloud.com/reference/custom_events-create-definition)
* [Send a custom event](https://docs.ycloud.com/reference/custom_events-send-event)

{% hint style="info" %}
When the send-event API returns `200`, it means YCloud has successfully received the event.
{% endhint %}



**Option 3: Trigger by Conversation Keywords**

This option is suitable for scenarios where you want to identify high-intent leads based on what customers explicitly say in WhatsApp conversations.

1. In `Event Type`, select `System Events - Keywords`.
2. Add one or more keywords.
3. Select the TikTok event to report, and turn on `Send to TikTok` if needed.
4. Save the rule.

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2FjGpLoTOZaJWMEOrYHOGe%2Fchooose-eventtype-keyword%3Avalue-t1.png?alt=media&#x26;token=9e088950-62d1-4091-a0fc-5f24ec1f2c46" alt=""><figcaption></figcaption></figure>

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2Fj0opP799gOUNBkGCJP9q%2Fchooose-eventtype-keyword%3Avalue1.png?alt=media&#x26;token=d493797e-9a50-49da-afc8-79743b63ee12" alt=""><figcaption></figcaption></figure>

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2FzU6ZlSBPuVTOJexLTL1Q%2Ftrackevents-list-keywords-t1.png?alt=media&#x26;token=8deec69b-8a92-40a0-a90f-da7fdd98ab78" alt=""><figcaption></figcaption></figure>

When a contact has recently clicked a relevant ad and their WhatsApp message contains any of the keywords you defined, YCloud will recognize the action as a conversion and decide whether to send it back to TikTok based on your rule.

{% hint style="info" %}
Keyword-based triggering is useful for identifying high-intent leads, but it may also result in false positives. We recommend using only keywords with clear business meaning.
{% endhint %}

### 3、 View Ad Performance and Conversion Data

After your ads start running, you can view ad performance, conversation data, and conversion data in both TikTok Ads Manager and YCloud.

#### View Data in TikTok Ads Manager

You can view performance data for campaigns, ad groups, or ads in the Campaign module, including spend, impressions, clicks, conversations, and other metrics.

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2FbFLJKRVbUyRDrKbhw3Wv%2Ftiktok%E5%B9%BF%E5%91%8A%E5%90%8E%E5%8F%B0-%E5%B9%BF%E5%91%8A%E5%88%97%E8%A1%A8-t1.png?alt=media&#x26;token=0b9d23e9-2926-4417-936b-dbbf8ee32605" alt=""><figcaption></figcaption></figure>

You can also view event data reported by YCloud in TikTok's event data pages.

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2F2ruEDPTsjp82RIQEDIao%2Ftiktok%E5%B9%BF%E5%91%8A%E5%90%8E%E5%8F%B0-eventmanager-datasource-%E6%95%B0%E6%8D%AE%E9%9B%86%E5%88%97%E8%A1%A8-t1.png?alt=media&#x26;token=0e31e421-b163-4a6e-898a-6744439028c0" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
In the data source list, some event sets are named `WhatsApp + [Phone Number]`. You can search by WhatsApp Business Number to find the corresponding data source.
{% endhint %}

After you click a messaging event set, you can view the historical events and related data reported by YCloud under that data source.

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2FCvvRowC3jkusHPvnb3Ct%2Ftiktok%E5%90%8E%E5%8F%B0-eventmanager-%E6%95%B0%E6%8D%AE%E9%9B%86%E8%AF%A6%E6%83%85-t1.png?alt=media&#x26;token=24717e9a-1ead-4f6d-864b-330bd0924ba3" alt=""><figcaption></figcaption></figure>

Among these events:

* The Conversation event is reported by YCloud by default.
* For any event other than Conversation, you must first configure the rule in Step 7 and turn on `Send to TikTok` before it will appear here.

#### View Data in YCloud

You can view ad performance and conversion data for a specific TikTok ad account in `CTWA > Ad Manage`.

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2Fx4GDtQvKWBTRaMhoaCTR%2Fctwa-ad_manage-tiktokad-t1.png?alt=media&#x26;token=17d01606-9a36-490b-8673-758659abc977" alt=""><figcaption></figcaption></figure>

If you need more detailed event records or lead data, go to `Track Events / View Leads`.

For a more complete explanation of the data, see: [CTWA Analytics](https://helpdocs.ycloud.com/help-center/ctwa-click-to-whatsapp-ad/ctwa-analysis)

### FAQ

<details>

<summary>Q: If `Send to TikTok` is turned off, will YCloud still record the data?</summary>

Yes. YCloud will still record the event, but it will not send the event back to TikTok.

</details>

<details>

<summary>Q: Why can I only see the Conversation event in TikTok, but not other conversion events?</summary>

Other than the Conversation event, all other events must first be configured in Step 7 and have `Send to TikTok` turned on before YCloud will send them back to TikTok.

</details>

