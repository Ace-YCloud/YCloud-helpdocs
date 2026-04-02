---
doc_id: doc_ctwa_click_to_whatsapp_ad_tiktok_messaging_ad_connect_tiktok_ad_account
language: zh-CN
title: "授权 TikTok 广告账户"
slug: connect-tiktok-ad-account
path: ctwa-click-to-whatsapp-ad/tiktok-messaging-ad/connect-tiktok-ad-account
document_group: ctwa-click-to-whatsapp-ad
path_in_group: tiktok-messaging-ad/connect-tiktok-ad-account
parent_id: doc_ctwa_click_to_whatsapp_ad_tiktok_messaging_ad
order: 0
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T07:22:50.568Z
updated_at: 2026-04-02T07:22:50.568Z
last_synced_at: 2026-04-02T07:22:50.568Z
tags:
---

# 授权 TikTok 广告账户

{% hint style="info" %}
开始前必读：[TikTok消息广告：流程指引、前期准备](./)。
{% endhint %}

### 第一步：在 YCloud 连接 TikTok 广告账户

在开始创建广告之前，您需要先在 YCloud 中完成 TikTok 广告账户授权。完成授权后，YCloud 才能识别您要用于投放的广告账户，并支持后续的号码绑定、消息事件集创建和事件回传。

#### 操作步骤

1. 在 YCloud 中-> CTWA，点击 Connect Ad Account (TikTok)

<figure><img src="../../.gitbook/assets/ctwa_initial_tk.png" alt=""><figcaption></figcaption></figure>



2. 在跳转后的 TikTok 授权页面中，登录您的 TikTok Ads 账户。

<figure><img src="../../.gitbook/assets/tiktok_ad-tiktok login (1).png" alt=""><figcaption></figcaption></figure>

3. 请确认您的 TikTok登陆账号后，请点击：确定，完成授权。

<figure><img src="../../.gitbook/assets/TIKTOK_ACCOUNT_OAUTH.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
如果发现您登录的TikTok账号是错误的，需要更换账号。请点击【切换账号】。
{% endhint %}



4. 返回 YCloud，此时广告账户应显示在账号列表中。

<figure><img src="../../.gitbook/assets/tiktok-account-connectedSuccessfully-popup.png" alt=""><figcaption></figcaption></figure>

* 如果您是第一次使用TikTok 消息广告，建议您跟随引导去完成设置。进入第二步
* 如果您的TikTok广告账号，已绑定过WhatsApp 商业号码，则选择跳过。进入第三步；

#### 注意事项

* 当前登录的 TikTok 账号需要对目标 Ad Account 拥有足够权限，否则可能出现授权不足或无法完成授权的问题。



### 第二步：在 YCloud 中绑定用于投放的 WhatsApp Business 号码

完成广告账户连接后，您需要在 YCloud 中为该广告账户选择用于投放的 WhatsApp Business 号码。

{% hint style="info" %}
绑定后，YCloud 会在 TikTok广告后台 为您创建该号码对应的消息事件集（又称Event Set）。\
您后续在TikTok广告后台，创建 TikTok 消息广告时会用到。
{% endhint %}



#### 操作步骤

您可以通过以下两种方式进入绑定流程：

1. TikTok 广告账户绑定成功后，按页面指引点击“立即绑定 WhatsApp 号码”。

<figure><img src="../../.gitbook/assets/tiktok-account-connectedSuccessfully-popup.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
选择跳过后。如果以后想关联新的WhatsApp商业号码，怎么办？

Ad Account -找到对应的广告账号 -点击 Event Set - 创建新的Event Set就可以绑定 WhatsApp Business 号码。
{% endhint %}

进入绑定流程后：

<figure><img src="../../.gitbook/assets/tiktok-popup2-create-Eventset-t1 (1).png" alt=""><figcaption></figcaption></figure>

1. 确认 Ad Account
2. 选择要用于投放的 WhatsApp Business 号码。
3. 提交配置并确认创建成功。

#### 注意事项

* 用于投放的 WhatsApp Business 号码必须已经接入 YCloud。
* 在同一个广告账户下，每个 WhatsApp Business 号码只需要绑定一次；
* 如果某个号码已经绑定到当前广告账户，系统会显示为 Used。

<figure><img src="../../.gitbook/assets/tiktok-popup2-number_is_invalid-t1.png" alt=""><figcaption></figcaption></figure>

