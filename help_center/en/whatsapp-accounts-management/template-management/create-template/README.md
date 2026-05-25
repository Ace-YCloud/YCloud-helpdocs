# Create Template

## Tutorial for Creating Marketing and Utility Templates

### Step 1: Access the Templates Page

1. Navigate to Templates from the left-hand navigation. Users with multiple WABA accounts should switch the WABA space in the top right corner.

<figure><img src="../../../.gitbook/assets/image (194) (1).png" alt=""><figcaption><p>Templates</p></figcaption></figure>

2. Enter Templates from the WhatsApp accounts.

<figure><img src="../../../.gitbook/assets/image (195) (1).png" alt=""><figcaption><p>WABA > Templates</p></figcaption></figure>

### Step 2: Name & Select Template Type

1. Template name: The name of the template. Names only support numbers, lowercase letters, and underscores \_.

{% hint style="info" %}
Note: The name is unique and is the name called when sending via the interface.
{% endhint %}

2. Category: The type of template. There are three types of templates, select based on the content:
   1. Utility: Transactional templates. Used for sending notification messages.
   2. Marketing: Marketing templates. All messages with marketing implications, as well as all greeting messages.
   3. Authentication: Verification code templates. Fixed content, only supports sending verification codes.

<figure><img src="../../../.gitbook/assets/image (198) (1).png" alt=""><figcaption><p>Template name &#x26; Category</p></figcaption></figure>

### Step 3: Choose Language

One template content can be configured in multiple languages. Click Add language to continue adding.

Multiple languages can be edited together and then submitted.

<figure><img src="../../../.gitbook/assets/image (197) (1).png" alt=""><figcaption><p>Choose language</p></figcaption></figure>

Click the Edit button on the right side of the language to edit or delete the language.

<figure><img src="../../../.gitbook/assets/image (199) (1).png" alt=""><figcaption><p>Edit language</p></figcaption></figure>

### Step 4: Edit Template Content

[View introduction to creating verification code templates](./#yan-zheng-ma-mu-ban-she-zhi-can-shu-jie-shao)

Taking **marketing** and **notification templates** as examples:

1. Header (optional): Header types supported: text, image, video, file.
2. Body (required): Text content. Supports emoji, bold, and other text styles.
3. Footer (optional): Text footer.
4. Button (optional)
   1. Up to 10 buttons can be added
   2. Button types include:
      1. Quick reply
      2. Visit website
      3. Call phone number
      4. Copy offer code
5. Variables: Variables can be added in Header, Body, or Visit website. When adding variables, a Sample must be provided for reviewers to judge the content of the entire template. The Sample is only used for review, and the actual variable value must be sent when issuing.

<figure><img src="../../../.gitbook/assets/image (4) (1).png" alt=""><figcaption></figcaption></figure>

Detailed template content can be found in the [Message Templates](../../../whatsapp-basics/message-templates/) documentation

<figure><img src="../../../.gitbook/assets/image (22) (1).png" alt=""><figcaption><p>Edit template</p></figcaption></figure>

### Step 5: Submit Template

After all languages are edited, scroll to the bottom of the page and click the submit button.

<figure><img src="../../../.gitbook/assets/image (23) (1).png" alt=""><figcaption><p>Submit template</p></figcaption></figure>

Confirm the template content is correct and click Confirm.

<figure><img src="../../../.gitbook/assets/image (24) (1).png" alt=""><figcaption><p>Confirm</p></figcaption></figure>

### Step 6: Wait for Approval

The template is reviewed by Meta, please be patient. Generally, the review will be completed within one day.

If the template is rejected, you can enter the edit page to view the reason, and modify the template or appeal according to the prompt.

<figure><img src="../../../.gitbook/assets/image (203) (1).png" alt=""><figcaption><p>Rejected template</p></figcaption></figure>

## Introduction to Creating Verification Code Templates

The steps to create verification code templates are the same as above, this section mainly introduces the settings for verification code templates.

### Code Delivery

Code delivery sets the method of delivering the verification code, with three options:

* [Copy Verification Code](./#fu-zhi-yan-zheng-ma-de-mu-ban)
* [One-Click Fill Verification Code](./#yi-jian-tian-chong-yan-zheng-ma)
* [Zero-Click Autofill Verification Code](./#ling-dian-ji-yan-zheng-ma-mu-ban)

#### Copy Verification Code Template

Choose the Copy Code type of sending method. You can customize the button name. [Click for detailed introduction](../../../whatsapp-basics/message-templates/authentication-message-templates/copy-verification-code-authentication-template.md)

<figure><img src="../../../.gitbook/assets/image (6) (1).png" alt=""><figcaption></figcaption></figure>

#### One-Click Fill Verification Code

Choose the Autofill type of sending method. You can customize the button name. The Autofill mode requires entering your App's Package name and App signature hash. The one-click fill verification code requires your application to be able to initiate a "handshake". [Click for detailed introduction](../../../whatsapp-basics/message-templates/authentication-message-templates/one-click-autofill-authentication-template.md)

<figure><img src="../../../.gitbook/assets/image (5) (1).png" alt=""><figcaption></figcaption></figure>

#### Zero-Click Verification Code Template

Choose the Autofill type of sending method. Complete the Autofill information configuration. Enable the Zero-tap button and agree to the protocol.

The zero-click verification code is an upgrade of the one-click fill verification code template, so it also requires your application to be able to initiate a "handshake". [Click for detailed introduction](./#ling-dian-ji-yan-zheng-ma-mu-ban)

<figure><img src="../../../.gitbook/assets/image (7) (1).png" alt=""><figcaption></figcaption></figure>

### Template Content Settings

Although the content of the verification code template is fixed, you can still add verification code validity and security tips through switches.

<figure><img src="../../../.gitbook/assets/image (8) (1).png" alt=""><figcaption></figcaption></figure>

### Verification Code Message Validity Time Configuration

Since WhatsApp business api messages are valid for 30 days, meaning that after sending, customers can open WhatsApp within 30 days to view the message, leading to successful receipt and charging. However, 30 days is too long for verification code messages, which are typically only valid for a few minutes. Therefore, WhatsApp provides a configuration for the validity time of messages in verification code templates.

**Function:** After this verification code template message is sent, if it is not successfully received within the set message validity time, it will not continue to try to send. That is, no fee will be incurred. **We strongly recommend setting the message validity time less than or equal to the actual validity time of your verification code**.

Example: _You configure the message validity time to be 5 minutes (the actual validity time of the verification code in your app might be 10 minutes)._

_WhatsApp sends the verification code message to the user, but due to the user being offline or other reasons, the message remains in the processing (sending) state for 5 minutes. After this duration, WhatsApp stops trying to send this message to the user, and no fee is incurred. Even if the user connects to the internet and opens WhatsApp after 5 minutes, they will not see this message._

Configuration entry:

<figure><img src="../../../.gitbook/assets/image (9) (1).png" alt=""><figcaption></figcaption></figure>

## Related Reading

{% content-ref url="../../../whatsapp-basics/message-templates/" %}
[message-templates](../../../whatsapp-basics/message-templates/)
{% endcontent-ref %}
