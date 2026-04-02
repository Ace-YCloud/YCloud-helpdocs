---
doc_id: doc_integrations_qu_dao_verify_yan_zheng_yan_zheng_zui_jia_shi_jian_fang_zhi_qi_zha_he_wu_xiao_zhu_ce
language: zh-CN
title: "防止欺诈和无效注册"
slug: fang-zhi-qi-zha-he-wu-xiao-zhu-ce
path: integrations/qu-dao/verify-yan-zheng/yan-zheng-zui-jia-shi-jian/fang-zhi-qi-zha-he-wu-xiao-zhu-ce
document_group: integrations
path_in_group: qu-dao/verify-yan-zheng/yan-zheng-zui-jia-shi-jian/fang-zhi-qi-zha-he-wu-xiao-zhu-ce
parent_id: doc_integrations_qu_dao_verify_yan_zheng_yan_zheng_zui_jia_shi_jian
order: 40
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T11:16:23.030Z
updated_at: 2026-04-02T11:16:23.030Z
last_synced_at: 2026-04-02T11:16:23.030Z
tags:
---

# 防止欺诈和无效注册

随着全球欺诈风险的增加，一些攻击者向特定号码发送大量短信或语音验证请求以牟利。此外，许多应用程序提供只有新用户才能享受的“福利”，攻击者通过各种方式批量注册虚假账户以获得奖励。

* 短信诈骗：诈骗者向特定移动网络运营商 (MNO) 控制的一系列号码发送短信，并分享由此产生的收入。
* 国际收入分成欺诈 (IRSF)：欺诈者以电话验证为目标，向优质电话号码拨打大量语音电话以赚取佣金。
* 虚假注册：攻击者利用脚本批量创建虚假账户，获取新用户奖励，然后套现。\
  他们的具体盈利方式可能有所不同，但都会导致你花额外的钱却得不到真正的用户。

&#x20;

## 如何判断自己是否受到攻击？

在意想不到的国家/地区，验证成功率/消息发送率迅速下降或验证数量突然增加。

&#x20;

## 建议措施

**在验证过程中部署检测机器人**

Google reCAPTCHA 等产品可以帮助检测和阻止机器人流量。例如，在每个 SMS OTP 请求之前执行检查以防止自动脚本和机器人程序。这将为合法用户带来最小的摩擦。

&#x20;

## 验证频率限制

限制验证请求的频率，以帮助防止欺诈并保护您的应用程序，例如：

* X 秒内每个号码最多请求 X 条验证消息
* 每个国家/地区在 X 秒内请求的最多 X 条验证消息
* 您甚至可以根据用户、IP 或设备标识符设计速率限制。

速率限制不能完全防止欺诈，但它们可以减慢攻击者的速度，使他们认为不值得攻击您的应用程序。

&#x20;

## 语音验证通道作为替代方案，仅在第三次尝试时可用

由于国际收入分成欺诈 (IRSF) 日益盛行，我们建议不要在开始时提供“给我打电话”选项，而应在尝试 3 次短信后才提供。

&#x20;

## 实施地理权限限制

您必须有明确的商业目的，因此来自其他国家/地区的验证请求应该受到怀疑。\
设置地理验证权限并禁用所有不打算发送消息的国家/地区，以防止恶意攻击者创建不必要的验证请求并浪费短信或语音费用。

&#x20;

## 发送前检查电话号码

发送前检查号码的线路类型。至少识别无效的固定电话和手机号码，并且仅向手机号码发送短信。

&#x20;

## 监控一次性密码 (OTP) 的验证成功率并创建警报

我们建议实时监控验证成功率的变化。如果您发现在意想不到的国家/地区验证成功率急剧下降或验证数量突然增加，您应该密切关注。它们可能来自一些恶意攻击者。\
我们建议设计一些触发警报，以在达到异常阈值时提醒您。YCloud verify内置安全警报触发器，您可以在界面上轻松配置，以接收异常警报。
