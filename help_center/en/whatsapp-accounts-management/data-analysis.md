# Data Analysis

The Data Analysis page integrates message records from all WABA numbers under the account.

## Message Delivery Statistics

Click on the left navigation Home > Analytics to enter the Data Analysis page. The default view shows message-level delivery statistics.

<figure><img src="../.gitbook/assets/image (732).png" alt=""><figcaption></figcaption></figure>

## Conversation Statistics

Switch to the Conversation tab to view conversation-level statistics.

{% hint style="warning" %}
Starting from July 1st, Meta has switched from conversation-based billing to message-based billing. Therefore, conversation-level statistics are only available for data before July 1st.
{% endhint %}

<figure><img src="../.gitbook/assets/image (301).png" alt=""><figcaption></figcaption></figure>

## Message Logs

Click Logs to view all message sending records. You can see the sending time, receiving time, and status of each message.

### Sending Records

User is the customer's number, and Account is the WhatsApp API account that sent the message.

<figure><img src="../.gitbook/assets/image (288).png" alt=""><figcaption></figcaption></figure>

### Receiving Records

Select Inbound message for Direction to view all received messages.

User is the customer's number, and Account is the WhatsApp API account that received the message.

<figure><img src="../.gitbook/assets/image (289).png" alt=""><figcaption></figcaption></figure>

## Frequently Asked Questions

<details>

<summary>Why is the message status Failed?</summary>

There are many reasons for a message to fail. Hovering over the question mark next to Failed will show the specific reason for the failure.

</details>

<details>

<summary>Why is the read time empty?</summary>

The read receipt is a toggle. If the customer has turned it off on their phone, no read status will be returned.

</details>

<details>

<summary>The Message does not display specific content, only shows prompts like [Button][Unsupported message]</summary>

Due to the rich variety of WhatsApp message styles, the log page cannot properly display some rich media messages and button interaction messages. You can copy the customer's phone number to the Inbox to search for their chat content.

</details>
