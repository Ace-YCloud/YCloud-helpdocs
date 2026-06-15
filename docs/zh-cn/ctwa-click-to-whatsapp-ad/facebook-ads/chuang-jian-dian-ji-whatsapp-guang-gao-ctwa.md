---
doc_id: doc_ctwa_click_to_whatsapp_ad_facebook_ads_chuang_jian_dian_ji_whatsapp_guang_gao_ctwa
language: zh-CN
title: "创建点击WhatsApp广告（CTWA）"
slug: chuang-jian-dian-ji-whatsapp-guang-gao-ctwa
path: ctwa-click-to-whatsapp-ad/facebook-ads/chuang-jian-dian-ji-whatsapp-guang-gao-ctwa
document_group: ctwa-click-to-whatsapp-ad
path_in_group: facebook-ads/chuang-jian-dian-ji-whatsapp-guang-gao-ctwa
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

# 创建点击WhatsApp广告（CTWA）

## 步骤1：通过YCloud创建WhatsApp Business API账户

您无法使用个人 WhatsApp 号码承接广告流量。在广告管理器中创建点击 WhatsApp 广告之前，请先通过 YCloud 创建 WhatsApp Business API 帐户。

👇 了解如何创建 WhatsApp Business API  帐户

{% embed url="https://helpdocs.ycloud.com/help-center/zh/whatsapp-accounts-zhang-hao-guan-li/chuang-jian-whatsapp-api-zhang-hao" %}





## 步骤2：将 WhatsApp Business API 号码连接到您的 Facebook 页面

Meta要求Facebook Page关联 WhatsApp API 账户后才可以创建点击 WhatsApp 广告：

* 确保你拥有Facebook Page的管理员权限
* 导航Facebook Page > 单击“设置”（右上角）>[ 选择 WhatsApp](https://www.facebook.com/settings?tab=linked_whatsapp)
* 输入您的 WhatsApp Business电话号码，然后点击“继续”
  * 若您的WhatsApp账号跟广告账户归属于同一个BM，可直接完成绑定
  * 若您的WhatsApp账号跟广告账户不属于同一个BM, 则重新登录WhatsApp的BM账号，访问[Request](https://business.facebook.com/settings/requests?)页面，批准绑定的请求

<figure><img src="../../.gitbook/assets/image (268).png" alt=""><figcaption></figcaption></figure>



_另外，如果您希望在 Instagram 上开展广告活动，您还应该将您的 Instagram 帐户与 Facebook 页面相关联。_

完成以上步骤后，您就可以开始设置您的第一个 Click-to-WhatsApp 广告了。

## 步骤3：在 Facebook 广告管理器上设置 Click-to-WhatsApp 广告

### 1.打开 Facebook 广告管理器

访问您的 Facebook 广告管理器并点击“[创建](https://www.facebook.com/micro_site/url/?click_from_context_menu=true\&country=apac\&destination=https%3A%2F%2Fbusiness.facebook.com%2Fads%2Fmanage%2Fpowereditor%2Fcreation\&event_type=click\&last_nav_impression_id=2mCEGZi42LXv9OX7S\&max_percent_page_viewed=66\&max_viewport_height_px=1166\&max_viewport_width_px=2282\&orig_http_referrer=https%3A%2F%2Fwww.twilio.com%2F\&orig_request_uri=https%3A%2F%2Fwww.facebook.com%2Fbusiness%2Fhelp%2F447934475640650%3Fid%3D371525583593535%26locale%3Den_US%26draft%3D447934475640650\&primary_cmsid=447934475640650\&primary_content_locale=en_US\&region=apac\&scrolled=true\&session_id=1XSz4ltobUuzllphE\&site=fb4b\&extra_data%5Bview_type%5D=v3_initial_view\&extra_data%5Bsite_section%5D=help\&extra_data%5Bplacement%5D=%2Fbusiness%2Fhelp%2F447934475640650)”即可开始。

### 2.选择营销活动目标

投放至WhatsApp，请选&#x62E9;**“互动”**

<figure><img src="../../.gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>

选择Manual sales campaign

<figure><img src="../../.gitbook/assets/image (158).png" alt=""><figcaption></figcaption></figure>

### 3.填写相关基础信息以创建您的广告系列。这包括：

* 为您的广告系列命名
* 声明您是否有特殊的广告类别，例如招聘
* 定义是否要对广告进行 A/B 测试
* 注意：该步骤中需要关闭Advantage+ catalog ads

<figure><img src="../../.gitbook/assets/image (275).png" alt=""><figcaption><p>创建广告系列</p></figcaption></figure>

### 4.配置广告组详细信息

* Conversion location：选择“Messaging apps”
* Ad type: Select "Click to message"
* Facebook Page: 选择 Facebook Page
* Messaging Apps: 选择 WhatsApp. 注意，不要选择其他message app例如：Messager
* Performance goal：选择Maximize number of purchases through messaging

{% hint style="info" %}
1. 只有完成上述[第 2 步](chuang-jian-dian-ji-whatsapp-guang-gao-ctwa.md#bu-zhou-2-jiang-whatsapp-business-api-hao-ma-lian-jie-dao-nin-de-facebook-ye-mian)[：将 WhatsApp Business API 帐户连接到您的 Facebook 页面后](chuang-jian-dian-ji-whatsapp-guang-gao-ctwa.md#bu-zhou-2-jiang-whatsapp-business-api-hao-ma-lian-jie-dao-nin-de-facebook-ye-mian)，您才会看到 WhatsApp 号码。
2. 广告只有在Performance goal 选择了 Maximize number of purchases through messaging时，才会根据YCloud回传的客户转化（Converted）数据自动优化投放。[点击了解CTWA 的客户转化追踪](../ctwa-fen-xi.md#ctwa-fen-xi-zi-ding-yi-gen-zong-shi-jian-1)


{% endhint %}



<figure><img src="../../.gitbook/assets/image (519).png" alt=""><figcaption><p>选择 WhatsApp 号码</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (159).png" alt=""><figcaption><p>选择performance goal</p></figcaption></figure>

### 5.选择您的受众、展示位置、预算和时间表

请参阅[Facebook 广告文档](https://www.facebook.com/business/tools/ads-manager)以全面了解出价策略。

现在您已成功选择了广告系列的目标和预算，请点击“下一步”并定义该广告系列的广告组。

### 6.设置广告创意

以下是优化广告创意和媒体展示位置以获得最佳效果的 5 点清单：

* 编辑 Facebook 和 Instagram 上的特定广告展示位置，以调整图像尺寸。您还可以一组图像转换为视频幻灯片以提高点击率。
* 为您的 Click To WhatsApp 广告添加主要文字和标题。您可以添加最多五个主要文本选项和标题。
* 向广告添加说明以获取更多详细信息和上下文。
* 为您的 WhatsApp 广告选择 CTA 按钮。您可以从多个可用的 CTA 中选择一个。
* 在高级预览中预览展示位置中的广告。这就是每个媒体展示位置在 Facebook 和 Instagram feed 上的外观。

### 7.创建和预览消息模板

点击“新建”并创建欢迎消息模板，以便在人们点击您的广告后快速聊天。

<figure><img src="../../.gitbook/assets/image (521).png" alt=""><figcaption><p>欢迎消息模板</p></figcaption></figure>

### 8.发布您的广告&#x20;

Facebook 现在将审核您的广告。一旦获得批准，它将根据您的定位上线。



### 常见问题

<details>

<summary><strong>Q1：创建广告时：在广告组-广告优化目标的选项中，没有 购物次数最大化 ？</strong></summary>

创建广告时，广告优化目标，一般包含3种：

1. 点击最大化
2. 对话数最大化
3. 购物次数最大化

如果您发现，没有该**购物次数最大化**，表示：

您还未上传过[转化(Converted)](../ctwa-fen-xi.md#id-2.-she-zhi-converted)数据。您可以选择其他的Goal进行投放，当回传的转化数据超过10个后，您可以新建或者修改当前广告，修改goal为 “Maximize number of purchases through messaging”

</details>

<details>

<summary>Q2：创建广告时：找不到FB主页/Instagram账号/Whatsapp商业号码？</summary>



</details>

