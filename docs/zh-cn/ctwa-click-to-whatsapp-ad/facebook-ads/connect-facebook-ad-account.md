---
doc_id: doc_ctwa_click_to_whatsapp_ad_facebook_ads_connect_facebook_ad_account
language: zh-CN
title: "连接Meta广告帐户"
slug: connect-facebook-ad-account
path: ctwa-click-to-whatsapp-ad/facebook-ads/connect-facebook-ad-account
document_group: ctwa-click-to-whatsapp-ad
path_in_group: facebook-ads/connect-facebook-ad-account
parent_id: doc_ctwa_click_to_whatsapp_ad_facebook_ads
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

# 连接Meta广告帐户

为您介绍：通过YCloud完成Meta 广告业务的配置，并推动上线。

{% hint style="info" %}
开始前必读：

[Meta CTWA广告：说明与前期准备。](./)
{% endhint %}

### 在 YCloud 连接 Meta 广告账户 <a href="#di-yi-bu-zai-ycloud-lian-jie-tiktok-guang-gao-zhang-hu" id="di-yi-bu-zai-ycloud-lian-jie-tiktok-guang-gao-zhang-hu"></a>

1. 登陆 YCloud 平台 -> CTWA，点击Connect Ad Account (Meta Ads)

<figure><img src="../../.gitbook/assets/ctwa_initial_meta.png" alt=""><figcaption></figcaption></figure>

* 如果您已经授权过任何广告账号，请在 CTWA -> Ad Account（广告账号列表）点击Connect Ad Account 发起新的授权流程。&#x20;

<figure><img src="../../.gitbook/assets/ctwa-ad account-list-initial.png" alt=""><figcaption></figcaption></figure>



2.  在跳转后的 Meta 授权页面中，登录您的 Meta 账号。&#x20;

    <figure><img src="../../.gitbook/assets/meta广告账号授权-0：登陆meta账号.png" alt=""><figcaption></figcaption></figure>
3. 选择您的BM账号，点 继续

&#x20;<img src="../../.gitbook/assets/meta-ad account-oauth-1 select bm.png" alt="" data-size="original">

4. 选择该BM下：要授权的广告账号（可多选），点 继续，完成授权。

&#x20;<img src="../../.gitbook/assets/meta-ad account-oauth3-select ad account(from the bm).png" alt="" data-size="original">

{% hint style="info" %}
如果您在同一个BM下，有多个广告账号。建议您

* 只勾选：这次新增的目标🎯广告账号。
* 已默认勾选的数据，**不要取消勾选**。

yi已勾选的广告账号，意味着 之前已被授权给YCloud。

在您确定：该广告账号后续不再使用时，才可以解除授权。
{% endhint %}



点击Got it，回到YCloud后台，

此时，会提示您：广告账号授权已完成.

### 查看已授权的广告账户

您可以在Ad account中查看已授权的广告账户。

<figure><img src="../../.gitbook/assets/meta ad account-connected successfully.png" alt=""><figcaption></figcaption></figure>



接下来

1. 步骤2：[创建Meta 点击WhatsApp广告（CTWA）](https://helpdocs.ycloud.com/help-center/zh/ctwa-click-to-whatsapp-ad/meta-ctwa-guang-gao/chuang-jian-dian-ji-whatsapp-guang-gao-ctwa)
2. 步骤3：[Meta广告：CAPI转化事件的设置与上报。](https://helpdocs.ycloud.com/help-center/zh/ctwa-click-to-whatsapp-ad/meta-ctwa-guang-gao/zhuan-hua-api-capi)
3. 步骤4：[在YCloud与广告流量对话](https://helpdocs.ycloud.com/help-center/zh/ctwa-click-to-whatsapp-ad/jie-dai-ctwa-de-fang-ke)



### 常见问题

<details>

<summary>Q1：准备连接Meta广告账号，但我找不到想授权的BM 或 广告账号？</summary>

发生原因：您登录的Meta账号，没有对应BM、广告账号的管理权限/

解决办法：

{% hint style="info" %}
先看下您的WABA 和广告账号，是否属于同一个BM。分情况来分析
{% endhint %}

当**广告账号和您的WABA在同一个BM**（Business portfolio）

BM的管理员登陆BM后台，将BM及对应广告账号，授权给你的Meta账号。



当**广告账号和您的WABA是 不同的BM**

{% hint style="info" %}
当通过代理帮您开Meta广告账户时，就属于这种情况。
{% endhint %}

假设：

* BM-1：您公司的WABA归属于这个BM。
* BM-2：**代理的BM**。您找代理开通的广告账号，所有权归属于代理的BM。

操作授权办法

1.  步骤1：您登录BM-1后台，查找BM-1的业务资产编号.&#x20;

    <figure><img src="../../.gitbook/assets/meta-bm-overview-1.png" alt=""><figcaption></figcaption></figure>

提供ID给代理。



2. 步骤2：代理登陆BM-2后台，将资产授权给BM-1

<figure><img src="../../.gitbook/assets/meta-bm-userspartners-entrance-t1.png" alt=""><figcaption></figcaption></figure>

代理登陆BM-2后台，将资产：**广告账号授权给BM-1**（注：**必须勾选Full control 权限**/完全控制）&#x20;

<figure><img src="../../.gitbook/assets/meta-bm-userspartners-add permission-ad account-t1.png" alt=""><figcaption></figcaption></figure>



3. 步骤3：确保您已有BM-1的所有权或管理权，则可按流程授权广告账号。

如果您的Meta账号没有权限，请让BM-1的管理员登陆BM后台，在user/people为您的Meta账号开通广告账号的权限。



</details>

<details>

<summary>Q2：进入CTWA页面时，提示我需要绑定WABA号码</summary>

您需要前往：YCloud -> WhatsApp accounts 授权并绑定对应的WABA号码。

</details>

<details>

<summary>Q3：如何移除Meta广告账号对YCloud的权限？</summary>

{% hint style="info" %}
此操作，必须在Meta的BM后台进行设置。
{% endhint %}

在 Meta 商务管理平台 (BM) 中取消授权的步骤

1. 登录 [Meta 商务管理平台设置](https://business.facebook.com/settings/)。
2. 在左侧菜单栏选择 “用户” -> “系统用户”。
3. 找到 YCloud 使用的那个系统用户（通常名称包含 YCloud 或类似的标识）。
4.  在右侧的资产列表中，找到你目前绑定的那个“广告账号”，点击其旁边的 “X” 或 “移除”。

    > 注意：&#x20;
    >
    > 1. 这样 YCloud 就失去了对旧账号的访问权限，后续不会再产生数据关联。
    > 2. 后续如果要再使用该广告账号，需要再次授权

</details>
