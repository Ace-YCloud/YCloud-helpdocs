# Automation

Automation is the configuration for phone numbers, including:

* [Welcome message](automation.md#welcome-message-huan-ying-xiao-xi) (Feature Deprecation)
* [Ice breaker](automation.md#ice-breakers-po-bing-ti-shi)
* [Auto-reply for unassigned conversation](automation.md#autoreply-for-unassigned-conversations-zi-dong-hui-fu-wei-fen-pei-dui-hua)
* [Auto-reply for in queue conversations](https://helpdocs.ycloud.com/help-center/whatsapp-accounts-zhang-hao-guan-li/shou-ji-hao-ma-guan-li/zi-dong-hua#auto-reply-for-in-queue-conversations)
* [Auto-reply for delayed agent responses](automation.md#autoreply-for-delayed-agent-responses-chao-shi-zi-dong-hui-fu)
* [Auto-close Inbox conversations](automation.md#autoclose-inbox-conversations-chao-shi-zi-dong-guan-bi-dui-hua)
* [CSAT](https://helpdocs.ycloud.com/help-center/whatsapp-accounts-zhang-hao-guan-li/shou-ji-hao-ma-guan-li/zi-dong-hua#csat-customer-satisfaction)

Automation settings guidance: \
Home > WhatsApp accounts > Number's Settings > Automation

<figure><img src="../../.gitbook/assets/image (217).png" alt=""><figcaption><p>Automations</p></figcaption></figure>



## Welcome message (Feature Deprecation)

**Timing of sending**: Whenever a WhatsApp user fist opens a chat window with you.

{% hint style="info" %}
Note: It is triggered when the customer first opens a chat window with you, even before they send any message to you.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (218).png" alt=""><figcaption><p>Welcome message</p></figcaption></figure>

**Message format**: Welcome messages can be sent in free-form: text, media, interactive messages with buttons. _For example: Media message, see the example below:_

<figure><img src="../../.gitbook/assets/image (219).png" alt=""><figcaption><p>Media message as Welcome message</p></figcaption></figure>

**Use case**: Welcome messages are great for service interactions, such as customer support. For example, you can embed a WhatsApp button on your app or website. When a user clicks on the button, they are directed to WhatsApp, where they will receive a welcome message providing context on how to interact with you.

**Charges**: Although welcome messages are proactively sent by the business, the messages sent will be charged as service conversation type.

### Steps

#### Step 1: Enable the welcome message switch

<figure><img src="../../.gitbook/assets/image (220).png" alt=""><figcaption><p>Enable welcome message</p></figcaption></figure>

#### Step 2: Edit the auto-reply message content

Supported message types:

* Text message: Pure text type message. Supports Emoji, bold, italic, etc.
* Rich media message: Image/video/file + text type message.
* Interactive message: Interactive messages with buttons, such as quick reply buttons, view website buttons, list buttons.

{% hint style="info" %}
Note: For interactive messages, if you want to use list buttons, the Header must be set to None or plain text Header.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (221).png" alt=""><figcaption><p>Save welcome message</p></figcaption></figure>



## Ice breakers

Ice breakers provide users with a way to start a conversation with a business through a list of common questions. When a user opens your chat window, a list of preset ice breaker phrases will appear in the user's input box, and the user can send a message immediately by clicking on it.

<figure><img src="../../.gitbook/assets/image (222).png" alt=""><figcaption><p>Ice breakers</p></figcaption></figure>

**Rules**: You can configure up to 4 ice breakers on a phone number. Each ice breaker can have up to 80 characters. Emojis are not supported.

### Steps

#### Step 1: Enable the ice breaker switch

<figure><img src="../../.gitbook/assets/image (223).png" alt=""><figcaption><p>Enable ice breaker</p></figcaption></figure>

#### Step 2: Set options

After setting the options, click Save.

<figure><img src="../../.gitbook/assets/image (224).png" alt=""><figcaption><p>Edit and save Ice breaker</p></figcaption></figure>

## Auto-reply for unassigned conversations

When a conversation enters unassigned, which means no one is serving the conversation, the system automatically replies to the customer with a message to ensure timely response.

<figure><img src="../../.gitbook/assets/image (236).png" alt=""><figcaption><p>Auto-reply for unassigned message</p></figcaption></figure>

### Steps

#### Step 1: Turn on the switch

<figure><img src="../../.gitbook/assets/image (225).png" alt=""><figcaption><p>Enable auto-reply for unassigned conversations</p></figcaption></figure>

#### Step 2: Edit the auto-reply content

Click the Edit button to edit. Supported message types:

* Text message: Pure text type message. Supports Emoji, bold, italic, etc.
* Rich media message: Image/video/file + text type message.
* Interactive message: Interactive messages with buttons, such as quick reply buttons, view website buttons, list buttons.

After setting, click Save.

<figure><img src="../../.gitbook/assets/image (235).png" alt=""><figcaption><p>Edit and save auto-reply for unassigned conversations</p></figcaption></figure>

## Auto-reply for in queue conversations

When this switch is turned on, conversations in the queue will receive an automatically sent message, notifying the customer that they are currently in a waiting state, ensuring timely responses.

If a staff member who has reached their reception limit closes one of their ongoing conversations, a conversation from the queue will automatically be assigned to their inbox.

Additionally, staff members can also manually claim conversations that are in the queue.



### Steps

**Method 1:**

When the reception limit is reached, the number of people currently in the queue will be displayed at the top of the staff member's Inbox interface. Click on **people in queue**, select the conversation you want to transfer to yourself, and the transfer will be successful.

<figure><img src="../../.gitbook/assets/image (187).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (188).png" alt=""><figcaption></figcaption></figure>

**Method 2:**

Inbox > Unassigned > In queue

You can view the conversations currently in the queue. Click into a conversation to transfer it.

<figure><img src="../../.gitbook/assets/image (189).png" alt=""><figcaption></figcaption></figure>

## Auto-reply for delayed agent responses

If the customer's message is not replied to by the agents within the specified time, the system will automatically send a message to the customer. You can set the waiting time for sending reminder messages.

### Steps

#### Step 1: Turn on the switch

<figure><img src="../../.gitbook/assets/image (237).png" alt=""><figcaption><p>Enable Auto-reply for delayed agent responses</p></figcaption></figure>

#### Step 2: Set the waiting time and reply content

Waiting time: If the agent has not replied to the customer within the set time, the system will automatically reply.

Click the Edit button to edit the content. Supported message types:

* Text message: Pure text type message. Supports Emoji, bold, italic, etc.
* Rich media message: Image/video/file + text type message.
* Interactive message: Interactive messages with buttons, such as quick reply buttons, view website buttons, list buttons.

After setting, click Save.

<figure><img src="../../.gitbook/assets/image (238).png" alt=""><figcaption><p>Edit and save Auto-reply for delayed agent responses</p></figcaption></figure>

## Auto-close Inbox conversations

In the case of agent is serving the conversation, if the customer does not reply within the set time, the system will automatically close the conversation. You can set the auto-close time.

{% hint style="info" %}
This setting does not apply to unassigned conversations and conversations assigned to bots. Unassigned conversations will not be automatically closed, and conversations assigned to bots have two closing methods:

1. Close the conversation after the process is completed.
2. Close the conversation if the customer does not respond to the bot for 10 minutes.
{% endhint %}

### Steps

#### Step 1: Turn on the switch

<figure><img src="../../.gitbook/assets/image (239).png" alt=""><figcaption><p>Enable auto-close Inbox conversation</p></figcaption></figure>

#### Step 2: Edit the auto-close time

Supported configuration range: 1 minute to 72 hours.

Recommended configuration parameter: 24 hours.

After configuration, click Save.

<figure><img src="../../.gitbook/assets/image (240).png" alt=""><figcaption><p>Save auto-close Inbox conversations</p></figcaption></figure>

## CSAT（Customer Satisfaction)

When this switch is turned on, after a conversation handled by a human agent ends, a satisfaction survey will automatically be sent to the user. Please note that if the conversation is handled by a BOT, the satisfaction survey will not be triggered. **This feature is only effective for conversations handled by human agents.**

### Steps

#### Step 1: Turn on the switch

<figure><img src="../../.gitbook/assets/image (557).png" alt=""><figcaption></figcaption></figure>

**Step 2: Edit the Content**\
As shown in the image below, you can configure the text for the message and the button. Once the button is expanded, the survey format is fixed and cannot be modified.

<figure><img src="../../.gitbook/assets/image (558).png" alt=""><figcaption></figcaption></figure>
