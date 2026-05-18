---
description: 通过YCloud 管理您的Whatsapp 联系人
---

# 联系人管理

联系人用于统一管理客户资料、来源信息和后续运营信息。通过联系人列表，你可以查看客户从哪里进入、搜索联系人，并结合筛选条件对联系人进行分类管理。

### 联系人进入的条件

联系人可以通过以下方式进入 YCloud：

#### 手工导入

你可以通过手工方式添加联系人：

* [单个手工导入](https://helpdocs.ycloud.com/help-center/zh/contact/xin-jian-dao-ru-lian-xi-ren)
* [批量手工导入](https://helpdocs.ycloud.com/help-center/zh/contact/xin-jian-dao-ru-lian-xi-ren)

#### 接口导入

你也可以通过 API 创建联系人。点击查看 [接口导入](https://docs.ycloud.com/reference/contact-create) 文档。

#### 上行消息进入

当客户发送上行消息时，YCloud 会自动将他们的手机号码和姓名保存在你的账号 Contact 列表中，便于你后续对联系人进行管理。

#### 其他来源进入

联系人也可能来自链接、二维码、广告、帖子、Shopify、TikTok 广告、WhatsApp Business App 或通话等入口。

这些来源会记录在联系人属性中的“来源”字段中。你可以在联系人详情或联系人筛选条件中查看和使用该字段。

### 筛选联系人

Contact 支持按过滤器对联系人进行 segment 操作，便于对 Contact 列表进行高效分类管理。

你可以根据以下信息筛选或搜索联系人：

* 昵称
* 手机号
* 国家 / 地区
* 来源
* 标签
* 创建时间
* 最后联系时间

如果你需要了解“来源”“标签”“创建时间”“最后联系时间”等字段的含义，或需要配置自定义联系人属性，请参考 [联系人属性设置](https://helpdocs.ycloud.com/help-center/zh/contact/lian-xi-ren-she-zhi/lian-xi-ren-shu-xing-she-zhi)。

### 联系人详情

登录 [YCloud 账号](https://www.ycloud.com)，导航至 **Contact > Contact list**，可查看你的联系人列表。你也可以根据昵称、国家 / 地区等参数搜索联系人。

<figure><img src="../.gitbook/assets/image (919).png" alt=""><figcaption></figcaption></figure>

进入联系人详情后，你可以查看该联系人的基础资料、来源、标签和互动信息。常见信息包括：

* 昵称
* 手机号
* 邮箱
* 国家 / 地区
* 来源
* 标签
* 创建时间
* 最后联系时间
* 最后联系的号码

{% hint style="info" %}
联系人详情中展示的字段来自联系人属性。

* 系统属性由 YCloud 自动生成或更新
* 自定义属性可在联系人属性设置中配置。
{% endhint %}
