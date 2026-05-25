# Coupon Tool Usage

Manage promotional activities for businesses. Businesses can upload their own coupon codes and restrict each customer to claim only one coupon code. Uploaded coupon codes can be distributed in ChatBot, Inbox, and Campaign.

## Usage Scenarios

Scan to claim a coupon, where customers use a QR code to claim a coupon in your business account.

## Tutorial

### Step 1: Create a Coupon Campaign

#### Step 1.1: Enable Coupon Functionality

Entry: [Integrations](https://www.ycloud.com/console/#/app/integrations/all), click the Install button to enable

<figure><img src="../../.gitbook/assets/image (492).png" alt=""><figcaption></figcaption></figure>

#### Step 1.2: Create a Coupon Campaign

Navigate from the left sidebar Integrations > [Coupons](https://www.ycloud.com/console/#/app/integrations/coupon/list) to the Coupons page

Click \[+ New Coupons]

<figure><img src="../../.gitbook/assets/image (493).png" alt=""><figcaption></figcaption></figure>

#### Step 1.3: Configure Campaign Information

* Coupon Type: Code type (coupon code). Currently, only this type is supported; for other types, please contact us.
* Campaign Name: Name of the coupon campaign
* Campaign Notes: Notes about the campaign, optional.
* Claim Limit: Each person is allowed to claim only once.
* Campaign Duration: Set the campaign time. Coupons will stop being sent outside this time range.

After confirming the information is correct, click Submit.

<figure><img src="../../.gitbook/assets/image (494).png" alt=""><figcaption></figcaption></figure>

#### Step 1.4: Upload Coupon Codes

Click the upload button

<figure><img src="../../.gitbook/assets/image (495).png" alt=""><figcaption></figcaption></figure>

Upload the coupon code spreadsheet. You can click the template button to download a template.

{% hint style="info" %}
Note: In the uploaded Excel spreadsheet, the Code must be in the first column. YCloud will automatically remove duplicate coupon codes.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (496).png" alt=""><figcaption></figcaption></figure>

After uploading, click Save

<figure><img src="../../.gitbook/assets/image (497).png" alt=""><figcaption></figcaption></figure>

### Step 2: Configure the Claim Process in Chatbot

#### Step 2.1: Create a Chatbot

If you already have a Chatbot, you can directly enter your existing Chatbot. If not configured yet, see the [Create a Chatbot](../../chatbot/create-a-chatbot.md) tutorial.

#### Step 2.2: Create a Flow

Select the Chatbot you need to configure and click the Create Flow button.

<figure><img src="../../.gitbook/assets/image (499).png" alt=""><figcaption></figcaption></figure>

#### Step 2.3: Configure Flow Keyword

Set the Keyword to the claim keyword.

Example: If you want customers to receive a coupon when they hit "**Claim New User Coupon**", set the Keyword to **Claim New User Coupon**.

<figure><img src="../../.gitbook/assets/image (498).png" alt=""><figcaption></figcaption></figure>

#### Step 2.4: Configure the Sent Coupon

Add a Send message component in the Flow

<figure><img src="../../.gitbook/assets/image (10) (1).png" alt=""><figcaption></figcaption></figure>

In the message, click the coupon variable and select the coupon campaign to insert.

<figure><img src="../../.gitbook/assets/image (11) (1).png" alt=""><figcaption></figcaption></figure>

After editing successfully, link the Keyword and Send message components. Then save the Flow

<figure><img src="../../.gitbook/assets/image (13) (1).png" alt=""><figcaption></figcaption></figure>

### Step 3: Generate a QR Code for Sharing (Optional, only for QR code claim scenario)

Generate a QR code for the number, set the keyword to: **Claim New User Coupon**. [See detailed chat link configuration tutorial](../../whatsapp-accounts-management/phone-number-management/chat-links.md)

<figure><img src="../../.gitbook/assets/image (15) (1).png" alt=""><figcaption></figcaption></figure>
