---
doc_id: doc_integrations_qu_dao_quan_qiu_duan_xin_duan_xin_gong_neng_smpp
language: zh-CN
title: "SMPP"
slug: smpp
path: integrations/qu-dao/quan-qiu-duan-xin/duan-xin-gong-neng/smpp
document_group: integrations
path_in_group: qu-dao/quan-qiu-duan-xin/duan-xin-gong-neng/smpp
parent_id: doc_integrations_qu_dao_quan_qiu_duan_xin_duan_xin_gong_neng
order: 0
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T07:27:42.922Z
updated_at: 2026-04-02T07:27:42.922Z
last_synced_at: 2026-04-02T07:27:42.922Z
tags:
---

# SMPP

[SMPP](https://smpp.org/)是发送和接收 SMS 的行业标准。请联系我们的客户服务以启用此功能。

&#x20;

## &#x20;获取SMPP账户

请联系客服创建您自己的 SMPP 帐户。

&#x20;

## SMPP 的使用

### 连接

请连接以下服务器：

| 服务器地址           | 服务器端口 | SSL 服务器端口 |
| --------------- | ----- | --------- |
| smpp.ycloud.com | 30002 | 30012     |

联系我们以检索我们的公共证书。

###

### 装订

要发送绑定请求，请联系我们以检索您的 SMPP 系统 ID 和密码。

| 地位 | 描述               |
| -- | ---------------- |
| 0  | 成功               |
| 3  | SMPP 系统 ID 和密码无效 |
| 5  | 超过连接数限制          |

### &#x20;

### 提交消息

| 地位 | 描述      |
| -- | ------- |
| 0  | 成功      |
| 4  | 无效的电话号码 |
| 6  | 超过连接数限制 |

&#x20;

### 交货报告

以下是“deliver\_sm”PDU 中“short\_message”参数的示例：

```javascript
id:11041301030001006668 sub:001 dlvrd:001 submit date:2111040501 done date:2111040501 stat:DELIVRD err:0 text:none
```

“提交数据”和“完成日期”是 UTC 时间。

发送时'err'为'0'，其他数值为：

| 错误码 | 描述                |
| --- | ----------------- |
| 3   | 余额不足              |
| 4   | 不允许使用敏感词          |
| 10  | 该电话号码已列入黑名单       |
| 18  | 签名无效。中国大陆短信需要签名   |
| 65  | 被我们拒绝，通常是针对中国大陆短信 |
