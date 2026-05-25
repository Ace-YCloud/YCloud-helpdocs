# Number Migration

Number migration refers to the process of transferring a WhatsApp API number between WhatsApp Business Accounts (WABA) while retaining its display name, quality rating, template message limits, Official Business Account status, and approved high-quality templates.

Typically, number migration will be happened when a customer wants to transfer their WhatsApp API number from one solution partner to another.

_For example: If you have already registered a WhatsApp API account with another service provider before using YCloud, you can consider migrating the number to a newly created WABA on YCloud to continue using it._



## Migration Preparation

1. Sign-up a YCloud account.
2. Completed the WABA creation.  Phone numbers can be migrated between 2 WABAs in the same BM account, so you need to create a new WABA for this BM account in YCloud. If you haven't done it, [click here to see how to create a WABA](create-waba-via-embedded-sign-up.md).
3. Turn off two-step verification for the number.

## Notes

1. The number being migrated must have passed the display name review and not be in the process of being modified.
2. Historical chat records will not be migrated. Please back up the records with your original service provider.
3. The number's quality, green tick, configuration, and other attributes will not change after migration.
4. All approved medium/high-quality templates under the WABA will be synchronized. Low-quality or unusable templates cannot be synchronized. The quality rating of the templates will start from scratch after migration.

## Migration Process

### Step 1: Turn Off Two-Step Verification

Log in to the BM Account, Click WhatsApp account > Phone number, and turn off two-step verification. See below for more detailed steps.

Tip: If you did not register the original number yourself, please contact the registrant or administrator to turn it off.

#### Step 1.1: Enter the WABA Management Page

Visit the [Business Management Page](https://business.facebook.com/settings/whatsapp-business-accounts/), which needs to log in with the administrator's Facebook account before.

Select the WABA to which the number belongs > Settings > WhatsApp manager.

<figure><img src="../../.gitbook/assets/image (506).png" alt=""><figcaption><p>Business Manager settings</p></figcaption></figure>

#### Step 1.3: Enter the Phone Number Management Page

Click on the Phone numbers in the navigation bar, select the number to be migrated, and click the settings icon for the number.

<figure><img src="../../.gitbook/assets/image (30) (1).png" alt=""><figcaption><p>WABA settings</p></figcaption></figure>

#### Step 1.4: Turn Off Two-Step Verification

In the number management page, find Two-step verification and click Turn off two-step verification.

<figure><img src="../../.gitbook/assets/image (32) (1).png" alt=""><figcaption><p>Phone number settings</p></figcaption></figure>

After completing the above steps, you can proceed with the number migration process.

### Step 2: Migrate the phone number

#### Step 2.1: Visit WhatsApp accounts

Visit the [WhatsApp accounts](https://www.ycloud.com/console/#/app/dashboard/account) page and click Connect my WhatsApp account.&#x20;

<figure><img src="../../.gitbook/assets/image (158).png" alt=""><figcaption></figcaption></figure>

#### Step 2.2: Click Migrate phone number

<figure><img src="../../.gitbook/assets/image (159).png" alt=""><figcaption></figcaption></figure>

#### Step 2.3: Start migration

<figure><img src="../../.gitbook/assets/image (160).png" alt=""><figcaption></figcaption></figure>

#### Step 2.4: Confirm 2fa is disabled

<figure><img src="../../.gitbook/assets/image (161).png" alt=""><figcaption></figcaption></figure>

#### Step 2.5: Enter the phone number

<figure><img src="../../.gitbook/assets/image (162).png" alt=""><figcaption></figcaption></figure>

#### Step 2.6: Verify the phone number

Tip: For Mainland China (+86), it is recommended to use a voice call to receive the verification code.

<figure><img src="../../.gitbook/assets/image (163).png" alt=""><figcaption></figcaption></figure>



#### Step 2.7: Completed the migration

After the pop-up closes, YCloud will begin migrating the phone number. When we finish the process, the phone number will shown on this page and its status will show as Connected.

If the migration fails, please contact customer service for assistance.
