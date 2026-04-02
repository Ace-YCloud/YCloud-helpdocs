---
description: 做好准备并验证您的 BM帐户，以便每天在 WhatsApp 上发送无限量的消息
---

# BM企业认证

BM企业认证是一个旨在验证 BM帐户是否属于真实组织的过程。\
如果您尚未完成 BM企业认证，您将在使用 WhatsApp Business API 时受到限制，包括：

* 每个电话号码在 24 小时内滚动向 250 位唯一客户发送业务发起的对话。
* 最多注册 2 个电话号码。

完成企业验证和[显示名称审核](https://helpdocs.ycloud.com/help-center/zh/whatsapp-ji-chu/shou-ji-hao-ma#xian-shi-ming-cheng)后，您的企业有机会可以快速打开限制：

* 将业务发起的对话扩展到更多客户：从 24 小时滚动期间的 1,000 个唯一客户开始，逐渐增加到每个电话号码 10,000、100,000 或无限制。
* 响应无限的客户发起的对话。
* 请求成为官方企业帐户 (OBA)。
* 注册额外的电话号码（每个 BM 最多 20 个）。

{% hint style="info" %}
自 2024 年 4 月起，在满足消息质量标准并完成显示名称审核后，企业可以在聊天中显示其名称，从而提高客户对其的信任度\*，而无需进行企业验证。请参考Meta文档：[https://developers.facebook.com/docs/whatsapp/messaging-limits#open-1k-conversations-in-30-days](https://developers.facebook.com/docs/whatsapp/messaging-limits#open-1k-conversations-in-30-days)

_\*请注意，此功能正在由 Meta 逐步推出。我们尚不清楚它是否会应用于企业。_
{% endhint %}



### 业务验证准备 <a href="#preparation-for-business-verification" id="preparation-for-business-verification"></a>

您需要提前准备好以下信息：

<table><thead><tr><th width="277">资料</th><th>要求</th><th>示例</th></tr></thead><tbody><tr><td><strong>官网</strong></td><td><ol><li>必须是HTTPS加密</li><li>网站中需要包含公司的名称</li></ol></td><td><p>网址示例：https://www.ycloud.com </p><p></p><p>网站包含公司名称示例：© 2024 YCloud International Pte. Ltd. All rights reserved</p></td></tr><tr><td><strong>包含企业法定名称的官方文件，例如：</strong>营业执照，公司章程或者企业税务登记证明</td><td>文件中必须包含公司完整的名称、公司地址。公司的电话号码</td><td><img src="../.gitbook/assets/image (33).png" alt="" data-size="original"></td></tr><tr><td><strong>公司网址同一域名的邮箱地址</strong></td><td>它将被用来接收一次验证邮件（通过域名认证或手机号认证的方式不需要，但一般情况下，我们建议通过邮箱认证）</td><td>service@ycloud.com</td></tr></tbody></table>





## 验证流程

如果您是 Meta Business Manager 帐户的管理员，您可以按照以下步骤开始验证您的业务：

### 1. 启动验证

转至商务管理平台的[“安全中心”部分。](https://business.facebook.com/settings/security)\
如果您没有看到“验证”按钮，请访问 YCloud 控制台并完成[嵌入式注册流程](../whatsapp-accounts-zhang-hao-guan-li/chuang-jian-whatsapp-api-zhang-hao/tong-guo-qian-ru-shi-zhu-ce-chuang-jian-waba.md)。

<figure><img src="../.gitbook/assets/image (553).png" alt=""><figcaption></figcaption></figure>

### 2. 提交组织基础信息

提供您的组织名称、地址、电话号码和网站。

{% hint style="info" %}
要求

* 您填写的公司名称/地址必须与证明文件上的名称/地址完全一致
* 公司的电话号码，若无法修改，请前往 [Business info](https://business.facebook.com/settings/info?) 中修改
* 提交的网站必须有证明域名所有权的文字内容，例如，在页脚处输入“所属于公司 ABC”，该公司名称与您填写的公司名称必须一致。
{% endhint %}

<figure><img src="../.gitbook/assets/image (554).png" alt=""><figcaption></figcaption></figure>

### 3. 选择一种验证方式

选择一种验证组织真实性的方式。以下为两种推荐的验证方式，二选一即可。

{% hint style="info" %}
最佳实践

* 首选电子邮件验证，但您的电子邮件地址后缀必须与提交的域名匹配（[www.mypage.com](http://www.mypage.com/) >> [alex@mypage.com](mailto:alex@mypage.com)）。
* [域验证](https://www.facebook.com/business/help/321167023127050)是验证您的业务的下一个选项。
{% endhint %}

#### 3.1 邮箱验证

&#x20;选择邮箱验证。输入完整的邮箱地址，收到验证码后完成邮箱验证。

<figure><img src="../.gitbook/assets/image (555).png" alt=""><figcaption></figcaption></figure>

#### 3.2 域认证

3.2.1 进入[域名认证页面](https://business.facebook.com/settings/owned-domains/)，添加域名。例如：ycloud.com

<figure><img src="../.gitbook/assets/image (35).png" alt=""><figcaption></figcaption></figure>

3.2.2 验证域名

复制 meta-tag 的代码，然后将其安装到网站的header中。

完成安装后点击该页面的Verify domain。

<figure><img src="../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>

3.2.3 回到验证BM的页面，选择域名验证。

<figure><img src="../.gitbook/assets/image (555).png" alt=""><figcaption></figcaption></figure>

### 4. 上传证明文件

#### 4.1 上传文件公司文件

该文件必须显示您公司的法定名称和地址，最好该文件中包含公司的电话号码。

<figure><img src="../.gitbook/assets/image (556).png" alt=""><figcaption></figcaption></figure>

#### 4.2 上传公司地址和电话的文件

⚠️该选项不一定会出现。请仔细阅读提示

情况1：出现选项，您上传的文件中是否包含公司地址<mark style="color:red;">或</mark>电话号码？

您的营业执照中一定是已经包含了地址的，请选择是。



情况2：出现选项，您上传的文件中是否包含公司地址<mark style="color:red;">和</mark>电话号码？

若您的营业执照中没有包含地址和电话。您需要提供一份资料，例如公司发票，税票等。这份资料中必须包含公司的完整名称和电话号码。



### 5.等待验证结果

提交验证后，最快 10 分钟、最长 14 个工作日即可做出决定。审核完成后，您会收到通知。如果您收到已通过验证的确认信息，则无需执行任何其他操作。



## 常见问题

<details>

<summary>无法通过验证或验证时间过长</summary>

这是一个完全由 Meta 管理的内部流程。作为 YCloud，我们无法检查或更新您的验证状态或加快流程。

如果您在提交验证后遇到问题，[请排查您的商家无法验证的原因](https://www.facebook.com/business/help/2342133782492969)。

</details>

<details>

<summary><strong>验证按钮不可用</strong></summary>

您可以通过YCloud先创建WABA，验证按钮就会出现。

</details>

<details>

<summary>BM企业认证和绿勾（OBA认证）是一回事吗？</summary>

不。[绿勾（OBA认证）](green-tick-verification.md)是WABA下的号码知名度认证。

</details>

## 观看教程演示视频👇

{% embed url="https://www.bilibili.com/video/BV1Mt8MzwEXN/?spm_id_from=333.1387.homepage.video_card.click" %}







### Facebook 官方文档 <a href="#official-facebook-documentation" id="official-facebook-documentation"></a>

有关BM企业认证流程的更多信息，请参阅 Facebook 官方文档：

{% embed url="https://www.facebook.com/business/help/2058515294227817?id=180505742745347https://www.facebook.com/business/help/1095661473946872?id=180505742745347https://www.facebook.com/business/help/159334372093366" %}
