---
description: 了解如何从头开始，创建一个meta的Whatsapp广告
---

# 创建点击WhatsApp广告（CTWA）



#### 步骤1：通过YCloud创建WhatsApp Business API账户

您无法使用个人 WhatsApp 号码承接广告流量。在广告管理器中创建点击 WhatsApp 广告之前，请先通过 YCloud 创建 WhatsApp Business API 帐户。

[👇 了解如何创建 WhatsApp Business API 帐户](../../kuai-su-ru-men/chuang-jian-whatsapp-business-api-zhang-hu.md)

#### 步骤2：将 WhatsApp Business API 号码连接到您的 Facebook 页面

Meta要求Facebook Page关联 WhatsApp API 账户后才可以创建点击 WhatsApp 广告：

* 确保你拥有Facebook Page的管理员权限
* 导航Facebook Page > 单击“设置”（左边）> Linked account >[ 选择 WhatsApp](https://www.facebook.com/settings?tab=linked_whatsapp)
* 输入您的 WhatsApp Business电话号码，然后点击“继续”
  * 若您的WhatsApp账号跟广告账户归属于同一个BM，可直接完成绑定
  * 若您的WhatsApp账号跟广告账户不属于同一个BM, 则重新登录WhatsApp的BM账号，访问[Request](https://business.facebook.com/settings/requests?)页面，批准绑定的请求

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2FqbDTIrbRKPfZTQVApdpw%2Fimage.png?alt=media&#x26;token=2a56dd7d-e273-4420-8cf3-e06dc0ef2e96" alt=""><figcaption></figcaption></figure>

_另外，如果您希望在 Instagram 上开展广告活动，您还应该将您的 Instagram 帐户与 Facebook 页面相关联。_

完成以上步骤后，您就可以开始设置您的第一个 Click-to-WhatsApp 广告了。

#### 步骤3：在 Facebook 广告管理器上设置 Click-to-WhatsApp 广告

**1.打开 Facebook 广告管理器**

访问您的 Facebook 广告管理器并点击“[创建](https://www.facebook.com/micro_site/url/?click_from_context_menu=true\&country=apac\&destination=https%3A%2F%2Fbusiness.facebook.com%2Fads%2Fmanage%2Fpowereditor%2Fcreation\&event_type=click\&last_nav_impression_id=2mCEGZi42LXv9OX7S\&max_percent_page_viewed=66\&max_viewport_height_px=1166\&max_viewport_width_px=2282\&orig_http_referrer=https%3A%2F%2Fwww.twilio.com%2F\&orig_request_uri=https%3A%2F%2Fwww.facebook.com%2Fbusiness%2Fhelp%2F447934475640650%3Fid%3D371525583593535%26locale%3Den_US%26draft%3D447934475640650\&primary_cmsid=447934475640650\&primary_content_locale=en_US\&region=apac\&scrolled=true\&session_id=1XSz4ltobUuzllphE\&site=fb4b\&extra_data%5Bview_type%5D=v3_initial_view\&extra_data%5Bsite_section%5D=help\&extra_data%5Bplacement%5D=%2Fbusiness%2Fhelp%2F447934475640650)”即可开始。

**2.选择营销活动目标**

投放至WhatsApp，请选&#x62E9;**“互动”**

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2FFzgOQ9MJAEZFluva8Bj0%2Fimage.png?alt=media&#x26;token=5cdb982c-f9cf-42c0-8eb4-9a6138197c0f" alt=""><figcaption></figcaption></figure>

选择 Manual sales campaign

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2FWFcO0BOs02DU8oMXQj0J%2Fimage.png?alt=media&#x26;token=e692e919-f1dd-4ca0-83be-a2f6f4353241" alt=""><figcaption></figcaption></figure>

#### 3.填写相关基础信息以创建您的广告系列。这包括：

* 为您的广告系列命名
* 声明您是否有特殊的广告类别，例如招聘
* 定义是否要对广告进行 A/B 测试
* 注意：该步骤中需要关闭Advantage+ catalog ads

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2FzBJDcqzVfavtcx3Cn3ij%2Fimage.png?alt=media&#x26;token=5c941b23-3d76-40cc-9463-658b4b0b6cf4" alt=""><figcaption><p>创建广告系列</p></figcaption></figure>

#### 4.配置广告组详细信息

* Conversion location：选择“Messaging apps”
* Ad type: Select "Click to message"
* Facebook Page: 选择 Facebook Page
* Messaging Apps: 选择 WhatsApp. 注意，不要选择其他message app例如：Messager
* Performance goal：选择Maximize number of purchases through messaging

{% hint style="info" %}
1. 只有完成上述第 2 步：将 WhatsApp Business API 帐户连接到您的 Facebook 页面后，您才会看到 WhatsApp 号码。
2. 广告只有在Performance goal 选择了 Maximize number of purchases through messaging时，才会根据YCloud回传的客户转化（Converted）数据自动优化投放。[点击了解CTWA 的客户转化追踪](https://helpdocs.ycloud.com/help-center/zh/ctwa-fen-xi#ctwa-fen-xi-zi-ding-yi-gen-zong-shi-jian-1)
{% endhint %}

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2Fe6wOAiovVVQwZhHAnZIE%2Fimage.png?alt=media&#x26;token=ff0d1a13-cdf2-4eaf-acc5-4da2b4d1d681" alt=""><figcaption><p>选择 WhatsApp 号码</p></figcaption></figure>

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2FMcF04NusKzb7m2l0OQri%2Fimage.png?alt=media&#x26;token=7d882a46-5e80-4cac-b717-d5b5ce3e517d" alt=""><figcaption><p>选择performance goal</p></figcaption></figure>

#### 5.选择您的受众、展示位置、预算和时间表

请参阅[Facebook 广告文档](https://www.facebook.com/business/tools/ads-manager)以全面了解出价策略。

现在您已成功选择了广告系列的目标和预算，请点击“下一步”并定义该广告系列的广告组。

#### 6.设置广告创意

以下是优化广告创意和媒体展示位置以获得最佳效果的 5 点清单：

* 编辑 Facebook 和 Instagram 上的特定广告展示位置，以调整图像尺寸。您还可以一组图像转换为视频幻灯片以提高点击率。
* 为您的 Click To WhatsApp 广告添加主要文字和标题。您可以添加最多五个主要文本选项和标题。
* 向广告添加说明以获取更多详细信息和上下文。
* 为您的 WhatsApp 广告选择 CTA 按钮。您可以从多个可用的 CTA 中选择一个。
* 在高级预览中预览展示位置中的广告。这就是每个媒体展示位置在 Facebook 和 Instagram feed 上的外观。

#### 7.创建和预览消息模板

点击“新建”并创建欢迎消息模板，以便在人们点击您的广告后快速聊天。

<figure><img src="https://4253554051-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F78HV6e8vN6mhwsbohgTK%2Fuploads%2Fb0l4JrnLFk16jWdcITQI%2Fimage.png?alt=media&#x26;token=ddc813d5-e7f6-49b7-b49c-fae3241d0fdd" alt=""><figcaption><p>欢迎消息模板</p></figcaption></figure>

#### 8.发布您的广告

Facebook 现在将审核您的广告。一旦获得批准，它将根据您的定位上线。

#### 常见问题

<details>

<summary><strong>Q：创建广告时：在广告组-广告优化目标的选项中，没有 购物次数最大化 ？</strong></summary>

创建广告时，广告优化目标，一般包含3种：

1. 点击最大化
2. 对话数最大化
3. 购物次数最大化

如果您发现，没有该**购物次数最大化**，表示：

您还未上传过[转化(Converted)](https://helpdocs.ycloud.com/help-center/zh/ctwa-fen-xi#id-2.-she-zhi-converted)数据。

解决办法：先选择【对话次数最大化】作为目标，当回传的转化数据超过10个（每周）后，meta会逐步为您开放【最大转化-purchase】选项。您再创建广告或修改广告目标。

</details>

<details>

<summary><strong>Q: 什么是 CTWA 广告中的消息模板（Message templates）？</strong></summary>

CTWA 广告中的消息模板，是用户点击 Facebook 或 Instagram 广告并跳转到 WhatsApp 后，用来引导用户发起第一条消息的开场设置。

<figure><img src="../../.gitbook/assets/ctwa-message templates-beautified.png" alt=""><figcaption></figcaption></figure>



在创建广告时，通常可以选择两种方式：

* Frequently asked questions：展示几个用户可以点击发送的问题。
* Pre-filled message：在 WhatsApp 输入框中预先填入一段文字，用户可以直接发送，也可以修改后再发送。

> 这里的消息模板，指的是 CTWA 广告创建流程中的开场对话设置，不是 YCloud 中用于主动发送通知、营销或验证码的 WhatsApp 消息模板。



**两种方式有什么区别？**

| 类型                         | 用户看到什么                | 适合场景                         | 设置建议                |
| -------------------------- | --------------------- | ---------------------------- | ------------------- |
| Frequently asked questions | 用户看到多个可点击的问题选项        | 希望用户主动选择咨询方向，例如价格、商品、配送、联系销售 | 设置 3-5 个最常见、最有价值的问题 |
| Pre-filled message         | WhatsApp 输入框中自动填入一段消息 | 希望用户直接发送固定意图，例如咨询某个活动、商品或服务  | 文案要短，直接说明用户的意图      |

**Frequently asked questions 适合什么时候使用？**

如果您希望先判断用户想咨询什么，可以使用 Frequently asked questions。

例如：

* I want to know the price
* Show me the product catalog
* Do you ship to my country?
* I want to talk to sales

这种方式适合：

* 商品或服务类型较多
* 需要区分询价、售前、售后或销售咨询
* 已配置 Chatbot，希望根据用户点击的问题进入不同回复流程
* 客服需要更快判断用户意图

设置时，建议只保留最重要的 3-5 个问题。问题越多，用户越难选择。

<figure><img src="../../.gitbook/assets/edit-message templates-Frequently asked questions-beautified.png" alt=""><figcaption></figcaption></figure>

**Pre-filled message 适合什么时候使用？**

如果您希望用户点击广告后直接发送一段固定内容，可以使用 Pre-filled message。

例如：

* Hi, I’m interested in this product. Can you tell me more?
* Hi, I want to know more about the promotion.
* Hello, I’d like to get a quote.

这种方式适合：

* 广告只推广一个明确的商品、活动或服务
* 不需要用户先选择问题，只希望尽快开始对话
* 希望用固定文案作为 Chatbot 触发词
* 希望降低用户输入成本，让用户直接点击发送

设置时，建议让预填文本和广告内容保持一致。用户点击的是折扣广告，预填文本就应围绕折扣；用户点击的是报价广告，预填文本就应围绕询价。

<figure><img src="../../.gitbook/assets/edit-message templates-beautified (1).png" alt=""><figcaption></figcaption></figure>

**应该选择哪一种？**

如果您刚开始使用 CTWA 广告，可以按广告目标选择：

| 广告目标          | 推荐方式                       | 原因                     |
| ------------- | -------------------------- | ---------------------- |
| 获取更多泛咨询       | Pre-filled message         | 用户只需点击发送，开聊成本最低        |
| 区分用户需求        | Frequently asked questions | 可以提前判断用户想问价格、商品、配送还是销售 |
| 推广单一商品或活动     | Pre-filled message         | 对话意图更集中，适合承接单一广告内容     |
| 配合 Chatbot 分流 | Frequently asked questions | 每个问题都可以对应不同自动回复或流程     |
| 用关键词触发自动化     | Pre-filled message         | 固定文本更容易作为触发条件          |

**最佳实践**

* 模板内容要和广告文案保持一致。广告主推折扣时，问题或预填文本应围绕优惠、价格或购买。
* 不要让用户看完后还要思考怎么开口。无论选择哪种方式，都要让第一条消息足够自然。
* Frequently asked questions 不要设置太多，建议 3-5 个。
* Pre-filled message 不要写太长，用户能一眼看懂并愿意发送即可。
* 如果使用 Chatbot，建议让问题选项或预填文本与自动回复触发条件保持一致。
* 发布广告前，使用预览功能检查用户点击广告后的 WhatsApp 开场效果。

</details>

