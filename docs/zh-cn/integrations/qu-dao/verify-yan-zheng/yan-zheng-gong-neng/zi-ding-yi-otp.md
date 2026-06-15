---
doc_id: doc_integrations_qu_dao_verify_yan_zheng_yan_zheng_gong_neng_zi_ding_yi_otp
language: zh-CN
title: "自定义OTP"
slug: zi-ding-yi-otp
path: integrations/qu-dao/verify-yan-zheng/yan-zheng-gong-neng/zi-ding-yi-otp
document_group: integrations
path_in_group: qu-dao/verify-yan-zheng/yan-zheng-gong-neng/zi-ding-yi-otp
parent_id: doc_integrations_qu_dao_verify_yan_zheng_yan_zheng_gong_neng
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

# 自定义OTP

如果您已经拥有用于生成和验证验证码的系统并希望继续使用它们，您可以将您的代码发送给我们并使用我们预先批准的消息模板以及文本和语音本地化选项。

**如何使用自定义代码？**\
要使用您自己生成的验证码，请将其包含在对发送验证请求 API 的调用中。

```javascript
{
"to": "+44868534958",
"channel": "SMS",
"code": "1234",
}
```



为保证用户认证准确可靠，建议使用验证码API提交用户提供的验证码。这种方法不仅可以让您监控验证的成功率，还可以为我们提供有关全球短信线路稳定性的宝贵信息。通过利用此 API，您可以为用户提供无缝且安全的身份验证过程。
