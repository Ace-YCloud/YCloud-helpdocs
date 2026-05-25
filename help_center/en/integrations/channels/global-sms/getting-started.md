# Getting Started

Short Message Service, commonly abbreviated as SMS, is the text messaging component in mobile phone and other mobile device systems. As one of the most important messaging channels, SMS has been providing services in various ways for decades, such as personal communication, authentication, marketing, and notifications.

## Before You Start

**Understanding YCloud SMS**: [YCloud supports SMS in over 200 countries, you can check the countries and prices on our website](http://www.ycloud.com/price)

**Charges**: SMS is charged by segments. When the characters in an SMS exceed the limit of one SMS, the SMS will be split into multiple SMS messages for sending, which we call segments. [You can check the SMS character limit here](sms-basic-principles.md).

**What SMS is Charged for?** SMS is charged when the status is {undelivered, delivered, processing}. For status explanations, click [here](sms-basic-principles.md).

## Getting Started

Before integrating SMS channels, you need to contact customer service to activate the SMS function.

After successful activation, you can see the SMS navigation in Integration.

<figure><img src="../../../.gitbook/assets/image (290).png" alt=""><figcaption></figcaption></figure>

## Trial Account Considerations

You should be aware of some limitations:

* The trial account only supports sending SMS to the phone number you registered with.
* As for the sender ID, you can only use the default sender ID provided by YCloud.
* You can test SMS from the [Getting Started page](https://www.ycloud.com/console/#/app/sms/getStarted) or [API documentation](https://ycloud.readme.io/reference/sms-send).

You can upgrade your account at any time by [topping up](https://www.ycloud.com/console/#/app/payments/buyCredits) to remove usage restrictions.

## Choose Your Preferred Way to Connect

1. [**HTTP API**](sms-features/api-interface.md): Using our REST API makes access easier and faster.
2. [**Bulk Messages**](sms-features/mass-messaging.md): Manually send bulk messages using ready-made tools.
3. [**SDK**](https://github.com/YCloud-CPaaS): Designed for quick and easy integration.
4. [**SMPP**](sms-features/smpp.md): Supports maintaining a continuous connection with the SMSC. Please contact our customer service for an SMPP account.

## View Sending Records

[Click to visit the sending records page](https://www.ycloud.com/console/#/app/integrations/sms/analytics/logs)

<figure><img src="../../../.gitbook/assets/image (294).png" alt=""><figcaption></figcaption></figure>
