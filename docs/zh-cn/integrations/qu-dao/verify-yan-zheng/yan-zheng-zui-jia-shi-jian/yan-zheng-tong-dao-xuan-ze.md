---
doc_id: doc_integrations_qu_dao_verify_yan_zheng_yan_zheng_zui_jia_shi_jian_yan_zheng_tong_dao_xuan_ze
language: zh-CN
title: "验证通道选择"
slug: yan-zheng-tong-dao-xuan-ze
path: integrations/qu-dao/verify-yan-zheng/yan-zheng-zui-jia-shi-jian/yan-zheng-tong-dao-xuan-ze
document_group: integrations
path_in_group: qu-dao/verify-yan-zheng/yan-zheng-zui-jia-shi-jian/yan-zheng-tong-dao-xuan-ze
parent_id: doc_integrations_qu_dao_verify_yan_zheng_yan_zheng_zui_jia_shi_jian
order: 0
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T07:27:54.996Z
updated_at: 2026-04-02T07:27:54.996Z
last_synced_at: 2026-04-02T07:27:54.996Z
tags:
---

# 验证通道选择

每个验证渠道都有其自身的优点和缺点。根据您业务开展的国家/地区选择合适的验证渠道，有助于提高验证流程的通过率，保障账户安全。许多公司提供多种验证方式供客户选择。

YCloud的验证API支持多种验证通道，您可以快速集成：

* 短信
* WhatsApp
* 嗓音
* 电子邮件

&#x20;

## 短信

SMS 是最流行的双因素身份验证 (2FA) 和一次性密码 (OTP) 渠道，因为全世界大多数人都可以无障碍地接收短信。Google 研究表明，短信是一种有效的身份验证形式，有助于“阻止 100% 的自动机器人、96% 的批量网络钓鱼攻击和 76% 的定向攻击”。

然而，由于短信依赖于世界各地运营商的通信网络，因此其传送能力和每次验证的成本取决于您业务运营的各个国家/地区的传送基础设施。在美国、英国和中国等国家，成本低且交付能力高，因此这可能不是问题。但在东南亚和南美洲的一些国家/地区，短信可能不是最具成本效益的选择。

其次，由于全球欺诈风险和恶意攻击者不断增加，如果你的应用缺乏有效的应对措施，可能会花费大量的消息成本而得不到真正的客户。了解防御措施。

&#x20;

## WhatsApp

WhatsApp 是全球 100 多个国家/地区最受欢迎的社交工具，每月有超过 20 亿人通过 WhatsApp 进行互动。您可以通过电话号码向相应的 WhatsApp 帐户发送验证消息。

作为验证通道，它具有与短信相同的优点，不受当地运营商基础设施的影响，不会对未发送的消息进行收费，并且不易受到电信网络欺诈的影响。在印度、印度尼西亚、中东和南美，我们建议您使用WhatsApp作为首选验证渠道，因为它可以提高您的整体验证转化率，而且价格便宜。在其他地区，它可以作为备用渠道对于短信。

YCloud verify WhatsApp 不是您必须从头开始构建的东西，而是允许您通过预先批准的 WhatsApp 共享电话号码立即开始发送 OTP，而无需消息数量和行业限制。

&#x20;

## 语音验证

语音验证通常用作短信身份验证的主要备份。尽管短信发送率在全球范围内有所不同，但语音验证在运营商网络上具有优先权。

在YCloud verify中，我们集成了200多个国家的语音网络，支持12种语言的本地化。

同样，它也可能受到攻击。国际攻击者将尝试向某些电话号码发起大量语音呼叫，以从中获利。

了解防御措施。

&#x20;

## 电子邮件

电子邮件也是一种常见的验证渠道，常用于账户注册激活和双因素身份验证。在美国、加拿大、欧洲等国家/地区，人们在日常生活和工作中经常使用电子邮件，并习惯于使用电子邮件地址作为账户名。在这种情况下，使用电子邮件作为主要验证渠道是一个正确的选择。

然而，电子邮件的缺点也很明显。在全球许多国家/地区，人们并不经常使用电子邮件，甚至可能没有安装相应的应用程序。另一个严重的问题是密码通常可以通过电子邮件重置。这意味着攻击者只需危害一个因素，即客户的电子邮件收件箱，即可接管相应的帐户。

&#x20;

**最后**\
还是不确定使用哪个渠道进行验证？[联系我们](https://www.ycloud.com/)。
