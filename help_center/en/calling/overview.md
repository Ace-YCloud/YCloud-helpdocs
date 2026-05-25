# Overview

WhatsApp Calling is a feature of the WhatsApp Business Cloud API that enables businesses to conduct voice calls (VoIP) directly through WhatsApp.

It supports two call types:

* Inbound calls: customer → business
* Outbound calls: business → customer



## Pricing

#### Inbound Calls

* Free — regardless of whether the business answers the call.

#### Outbound Calls

* Charged based on connected call duration.
* Billing unit: every 6 seconds (rounded up to 6 seconds).
* The rate depends on the country code of the customer’s phone number.



Example:

Indonesia rate: 0.0242 USD / minute

If a business places a call to an Indonesian user and ends the call after 9 seconds:

→ Billing = 2 units × 0.0242 USD/ 10 = 0.00484 USD<br>

👉 _Click_ [_here_](https://www.ycloud.com/pricing#price-table) _to view full country-level pricing._







## User-Initiated Calls (Inbound)

Customers can initiate a voice call to your business in three ways:

#### 1. Call Button on Your WhatsApp Business Profile

Enable the call icon displayed directly on your WhatsApp Business number.

<figure><img src="../.gitbook/assets/image (55).png" alt=""><figcaption></figcaption></figure>

#### 2. Call-In Link

Generate a call-in link and place it on your website, email, or WhatsApp messages.

Customers simply click to initiate a voice call.

<figure><img src="../.gitbook/assets/image (56).png" alt=""><figcaption></figcaption></figure>

#### 3. “Call In” Button Inside WhatsApp Messages

Add a call button inside messages to encourage fast and direct call-ins.

<figure><img src="../.gitbook/assets/image (57).png" alt=""><figcaption></figcaption></figure>

## Business-Initiated Calls (Outbound)

To use WhatsApp Calling, your business account must meet the following conditions:

1. The Business portfolio message limit must reach the 2,000 tier.
2. The phone number’s registered country must _<mark style="color:orange;">not</mark>_ be in the restricted regions:
   * United States (+1)
   * Canada (+1)
   * Turkey (+90)
   * Egypt (+20)
   * Vietnam  (+84)
   * Nigeria (+234)



To protect user privacy, businesses must obtain user permission before initiating an outbound call.

You can obtain permission by sending:

* A template message with a calling-request button
* An interactive message prompting the customer to authorize a call

Once the user grants permission, you may place outbound calls within the authorization window.



Example: Calling Request Template

<figure><img src="../.gitbook/assets/image (58).png" alt=""><figcaption></figcaption></figure>

###

##

## Getting Started with WhatsApp Calling

YCloud supports two integration methods: (Choose one; cannot be enabled simultaneously.)



#### 1. HTTPS API Integration

If you plan to integrate via API, please contact your YCloud representative to enable this functionality.

Reference API documentation: [👉🏻Click](https://docs.ycloud.com/reference/whatsapp-calling-examples)

#### 2. YCloud Platform Calling (Recommended)

The following guide is based on using the YCloud web platform.

##

### Enabling WhatsApp Calling on YCloud

Each business number can independently enable or disable the Calling feature.

Navigate to:&#x20;

WhatsApp Accounts → Number Settings → Calling

Toggle the WhatsApp Calling switch to activate.

<figure><img src="../.gitbook/assets/image (59).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (60).png" alt=""><figcaption></figcaption></figure>

##

### Displaying the Call Button on Your Number

Enable Call Icon Visibility to display the inbound call button next to your WhatsApp number, allowing customers to directly call your business.

<figure><img src="../.gitbook/assets/image (61).png" alt=""><figcaption></figcaption></figure>

##

### Outbound Calling Permissions

You can assign specific team members to use the business number for outbound calls.

Only authorized members can initiate outbound calls on the YCloud platform.<br>

> Note: This restriction applies only to outbound calling within the YCloud UI. If you are using API integration, this permission setting does not apply.

<figure><img src="../.gitbook/assets/image (62).png" alt=""><figcaption></figcaption></figure>



W
