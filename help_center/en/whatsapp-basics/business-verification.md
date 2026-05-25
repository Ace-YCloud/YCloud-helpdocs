---
description: >-
  Prepare and verify your BM account to send unlimited messages on WhatsApp
  daily.
---

# Business Verification

Business Verification is a process designed to verify whether a BM account belongs to a legitimate organization.\
If you have not completed Business Verification, there will have some restrictions when using the WhatsApp Business API, including:

* Each phone number can initiate conversations with 250 unique customers in a rolling 24-hour period.
* A maximum of 2 phone numbers can be registered.

After completing business verification and the [display name review](https://helpdocs.ycloud.com/help-center/whatsapp-ji-chu/shou-ji-hao-ma#display-name), your business has the opportunity to quickly lift the following restrictions:

* Expand business-initiated conversations to more customers: starting from 1,000 unique customers in a rolling 24-hour period, each phone number could gradually increasing to 10,000 > 100,000 > Unlimited.
* Respond to unlimited customer-initiated conversations.
* Request to become an Official Business Account (OBA).
* Register additional phone numbers (up to 20 per BM).

{% hint style="info" %}
Starting April 2024, after meeting message quality standards and completing the display name review, businesses can display their name in chats to enhance customer trust without business verification. Please refer to the Meta documentation: [https://developers.facebook.com/docs/whatsapp/messaging-limits#open-1k-conversations-in-30-days](https://developers.facebook.com/docs/whatsapp/messaging-limits#open-1k-conversations-in-30-days)

_\*Please note that this feature is being rolled out gradually by Meta. We are not yet sure if it will apply to businesses._
{% endhint %}

### Preparation for Business Verification <a href="#preparation-for-business-verification" id="preparation-for-business-verification"></a>



<table><thead><tr><th>Materials</th><th width="249">Requirement</th><th>Example</th></tr></thead><tbody><tr><td>An official website</td><td><ol><li>HTTPS encrypted</li><li>The company name is displayed on the website</li></ol></td><td><p>https://www.ycloud.com</p><p></p><p></p><p>Display the company name on the websit:</p><p>© 2024 YCloud International Pte. Ltd. All rights reserved</p></td></tr><tr><td><p><strong>An official document containing the legal name of the business.</strong> </p><ol><li>business license</li><li>company bylaws</li><li> Enterprise tax registration certificate.</li></ol></td><td>The file must include the full name of the company, its address, and its telephone number</td><td><img src="../.gitbook/assets/image (134).png" alt="" data-size="original"></td></tr><tr><td>Email address  (required when you choose to use email address for business verification)</td><td><p>Email's domain must be same as your website.</p><p></p><p>Aim to collect the verification code in order to prove that the website belongs to you.</p></td><td>service@ycloud.com</td></tr></tbody></table>

## Verification Process

If you are an admin of the Business Manager account, you can start verifying your business by following these steps:

### 1. Initiate Verification

Go to the [“Security Center”](https://business.facebook.com/settings/security) of the Business Manager platform.\
If you do not see the "Verify" button, visit YCloud and complete the [embedded sign-up process](../whatsapp-accounts-management/create-a-whatsapp-api-account/create-waba-via-embedded-sign-up.md).

<figure><img src="../.gitbook/assets/image (468).png" alt=""><figcaption></figcaption></figure>

### 2. Submit Organizational Information

Provide your organization's name, address, phone number, and website.

<figure><img src="../.gitbook/assets/image (469).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Best Practices

* The company name/address you fill in must match the name/address on the proof document.
* The phone number can be a personal mobile number (but the company cannot be verified by phone number in subsequent steps).
* The submitted website must have text content proving domain ownership, for example, by entering "belongs to company ABC" in the footer, which must match the company name you filled in.
{% endhint %}

### 3. Choose a Verification Method

Email Choose a method to verify the authenticity of your company: Email, Phone call, Text message, or Domain verification.

{% hint style="info" %}
Best Practices

* Recommend **email verification.** your email address's domain must match the submitted website's domain ([www.mypage.com](http://www.mypage.com/) >> [alex@mypage.com](mailto:alex@mypage.com)).
* **Domain verification** is the second recommended method of verification..
{% endhint %}

#### 3.1Email verification

<figure><img src="../.gitbook/assets/image (470).png" alt=""><figcaption></figcaption></figure>

#### 3.2 Domain verification&#x20;

Visit the [domain](https://business.facebook.com/settings/owned-domains/) verification page, and add a domain. eg. ycloud.com

<figure><img src="../.gitbook/assets/image (135).png" alt=""><figcaption></figcaption></figure>

Copy the meta-tag code and install it to the header of your website.

Click the "**Verify domain**" after completing the installation

<figure><img src="../.gitbook/assets/image (136).png" alt=""><figcaption></figcaption></figure>

Back to the Business verification page and choose the "Domain verification"

<figure><img src="../.gitbook/assets/image (137).png" alt=""><figcaption></figcaption></figure>

### 4. Upload Proof Documents

Upload documents to prove your business is registered. These documents must show your company's legal name and address or phone number.

<figure><img src="../.gitbook/assets/image (471).png" alt=""><figcaption></figcaption></figure>

### 5. Wait for Verification Results

After submitting for verification, a decision can be made in 2 working days generally. You will be notified once the review is completed. If you receive confirmation that you have passed verification, no further action is required.



## Watching the tutorial video👇

{% embed url="https://youtu.be/4h1DTozIEzU" %}





## Frequently Asked Questions

<details>

<summary>Unable to pass verification or verification takes too long</summary>

This is a fully internal process managed by Meta. As YCloud, we cannot check or update your verification status or expedite the process.

If you encounter issues after submitting for verification, [troubleshoot why your business cannot be verified](https://www.facebook.com/business/help/2342133782492969).

</details>

<details>

<summary><strong>Verification button not available</strong></summary>

You can create a WABA through YCloud first, and the verification button will appear.

</details>

<details>

<summary>Is BM Business Verification the same as the Green Tick Verification (OBA Verification )?</summary>

No. The [Green Tick Verification (OBA Verification)](green-tick-verification.md) is a number visibility verification under WABA.

</details>

### Facebook Documentation <a href="#official-facebook-documentation" id="official-facebook-documentation"></a>

For more information about Business Verification process, please refer to the Facebook official documentation:

{% embed url="https://www.facebook.com/business/help/2058515294227817?id=180505742745347https://www.facebook.com/business/help/1095661473946872?id=180505742745347https://www.facebook.com/business/help/159334372093366" %}
