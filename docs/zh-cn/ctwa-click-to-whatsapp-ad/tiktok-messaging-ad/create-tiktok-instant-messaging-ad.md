---
doc_id: doc_ctwa_click_to_whatsapp_ad_tiktok_messaging_ad_create_tiktok_instant_messaging_ad
language: zh-CN
title: "创建TikTok 消息广告"
slug: create-tiktok-instant-messaging-ad
path: ctwa-click-to-whatsapp-ad/tiktok-messaging-ad/create-tiktok-instant-messaging-ad
document_group: ctwa-click-to-whatsapp-ad
path_in_group: tiktok-messaging-ad/create-tiktok-instant-messaging-ad
parent_id: doc_ctwa_click_to_whatsapp_ad_tiktok_messaging_ad
order: 20
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T11:13:30.710Z
updated_at: 2026-04-02T11:13:30.710Z
last_synced_at: 2026-04-02T11:13:30.710Z
tags:
---

# 创建TikTok 消息广告



{% hint style="info" %}
1. 开始前必读：[TikTok消息广告](./)
2. 步骤1、2：[授权TikTok广告账户](tiktok-ad-introduction.md)
{% endhint %}

### 第三步：在 TikTok Ads Manager 中创建广告系列

请前往： [TikTok Ads Manager ](https://www.google.com.hk/aclk?sa=L\&pf=1\&ai=DChsSEwiqqPGDlqSTAxXSJEQIHZaLMzcYACICCAEQABoCZHo\&co=1\&ase=2\&gclid=CjwKCAjw1N7NBhAoEiwAcPchpxlUEiX0xNtEGzufuRo7Dte9ubCkvY0l-I0DfJ2nmK2LyYNsdT_SShoCIqUQAvD_BwE\&cid=CAASuwHkaAxSalI9c69vCXS9-Yn3cX42F1iH-x5j6X-Y7NhyjR4JCEL1VbSYzKNUigTMV2a6aAHcElfykAABTXlorVrcsTFTZ8eBFm888vunOUo4oUj-jWpmKSzKT0LNU9Mf9PdoRGQw8BKqdg7rq9WvP7D0gXgO2aqM9s9qn-oKkzwEvMJAb0Zc9cw1WSzF6EQGqNY4Mt0BqXkg2aJajTC5bt9zAf-uO5FU0gec2reCuGmgu79gq6AN_mEIvg1_\&cce=2\&category=acrcp_v1_32\&sig=AOD64_1g9VH9wQxe_RDC08ulqiBhxywWAw\&q\&nis=4\&adurl=https://getstarted.tiktok.com/ttvalue?irgwc%3D1%26afsrc%3D1%26irclickid%3DXK7TIP2wAxyZRu6W4BzY6TnuUkuzaH1RwyBsSU0%26lang%3Den-US%26gad_source%3D1%26gad_campaignid%3D23462953610%26gbraid%3D0AAAABClJOcVVlo2p9Uozdy1ANAF_0bVRL%26gclid%3DCjwKCAjw1N7NBhAoEiwAcPchpxlUEiX0xNtEGzufuRo7Dte9ubCkvY0l-I0DfJ2nmK2LyYNsdT_SShoCIqUQAvD_BwE\&ved=2ahUKEwi2uuuDlqSTAxXLHEQIHREPLc8Q0Qx6BAgaEAE)中,创建广告活动。

#### 操作步骤

1. 登录 TikTok Ads Manager，点击 创建广告。

<figure><img src="../../.gitbook/assets/tiktok广告后台-campaign新建入口-t1.png" alt=""><figcaption></figcaption></figure>

2. 在 Campaign objective 中选择 获取线索。

<figure><img src="../../.gitbook/assets/tiktok广告后台-新建campaign-选择推广目标-t1.png" alt=""><figcaption></figcaption></figure>

继续，进入广告组设置。



### 第四步：配置 Ad Group 并设置 WhatsApp 跳转

在 Ad Group 层级，您需要完成消息跳转方式、WhatsApp Business 号码和消息事件集的配置。

#### 操作步骤

<figure><img src="../../.gitbook/assets/tiktok广告后台-创建广告组-选择渠道和目标-t1.png" alt=""><figcaption></figcaption></figure>

1. 在渠道中 选择 **即时通讯应用**。
2. 在 目标中 选择 **会话数**。
3. 在事件-选择应用中，选择 **WhatsApp**。

<figure><img src="../../.gitbook/assets/tiktok广告后台-创建广告组-已输入wa号码+消息事件集-t1.png" alt=""><figcaption></figcaption></figure>



4. 填写投放的 **WhatsApp 商业号码**。

{% hint style="info" %}
输入号码时，请注意：**国家码是需要单独选择的**。

如果您的号码是+1234567。需要分别在2个框：选择+1 、填入 234567。
{% endhint %}

5. 号码输入后，TikTok会自动匹配**消息事件集（YCloud在第2步已为您创建**）。

{% hint style="info" %}
注意，如果在创建tiktok消息广告时，对流程中的 消息数据集（也叫event -set ）有疑问，可[点此查看](https://helpdocs.ycloud.com/help-center/zh/ctwa-dian-ji-whatsapp-guang-gao/tiktok-guang-gao/tiktok-ad-introduction)。
{% endhint %}

输入号码后，您可以点击**检查ID是否能正常打开**，使用**TikTok应用扫码** 体验跳转WhatsApp的交互。

<figure><img src="../../.gitbook/assets/tiktok广告后台-创建广告组-预览广告demo-t1.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
注意，

TikTok消息广告，在WhatsApp的欢迎语为固定文案，不支持广告主自定义。

该文案会跟随TikTok用户的语言设置，自动切换为其他语言。
{% endhint %}



7. 继续完成预算、投放时间、受众定向和版位等其他设置。完成 Ad Group 配置后，继续进入广告创意设置。

#### 注意事项

* 填写的 WhatsApp Business 号码必须与 YCloud 中已绑定的号码一致。
* 国家码和号码主体需要分别填写。

### 第五步：完成广告创意配置

按TikTok广告流程的交互和指引 完成信息的录入。

#### 操作步骤

1. 上传广告图片或视频素材。
2. 在 Text 字段中填写广告文案。
3. 在文案中清楚说明用户点击后将通过 WhatsApp 与商家开始沟通。
4. 预览广告展示效果，并确认跳转链路是否正确。
5. 确认无误后，点击 Publish all 提交广告。
6. 广告审核通过后，可打开开关，开始投放。

#### 注意事项

* 发布前建议完整预览一次跳转链路，确认最终进入的是正确的 WhatsApp 会话。



