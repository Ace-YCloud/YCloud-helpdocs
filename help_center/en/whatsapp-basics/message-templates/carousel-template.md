---
description: This document introduces the carousel template and its usage.
---

# Carousel Template

Carousel templates allow you to send a marketing template message with a set of Carousel cards that can be viewed in a horizontal scrolling view:

<figure><img src="../../.gitbook/assets/image (794).png" alt="" width="375"><figcaption></figcaption></figure>

When a user clicks on a store URL link provided by a merchant, they are redirected to their default browser, which causes them to leave WhatsApp. If you want users to view more products within WhatsApp, you can use a [Carousel template](https://developers.facebook.com/documentation/business-messaging/whatsapp/templates/marketing-templates/product-card-carousel-templates). Carousel templates are only available for marketing template messages.

### Carousel Media Cards

A Carousel template consists of body text and Carousel Media Cards. Each Carousel Media Card consists of a header, body text, and buttons. The rules for each component are as follows:

* The number of Carousel Media Cards is limited to 2 to 10.
* Header types can only be images or videos.

Each card must contain one "Visit Website" button. Users can optionally add one more button; button types include quick reply, make a phone call, and visit the website. Each card can contain a maximum of two buttons.

All cards added to a Carousel template must have the same component type, including the following rules:

* Header type.
* Number and type of buttons.

<figure><img src="../../.gitbook/assets/image (795).png" alt=""><figcaption></figcaption></figure>

### Create a Carousel template

You can create a Carousel template in YCloud's Template.

First, select the Media card carousel template in the Marketing Templates directory.

<figure><img src="../../.gitbook/assets/image (796).png" alt=""><figcaption></figcaption></figure>

Then, fill in the body text and cards in sequence.

Before filling in the cards, select the card format, such as: header , button.

⚠️ Please ensure that the media type you upload in each card title is consistent.

<figure><img src="../../.gitbook/assets/image (797).png" alt=""><figcaption></figcaption></figure>

💡 Once the template is approved, you can send this template message in 3 ways:

1. [Inbox: Send it to a contact](https://helpdocs.ycloud.com/help-center/inbox/initiate-new-chat)
2. [WhatsApp Campaign](../../campaign/create-a-whatsapp-marketing-campaign.md)
3. [API: Send it via API](https://docs.ycloud.com/reference/whatsapp_message-send-directly)
