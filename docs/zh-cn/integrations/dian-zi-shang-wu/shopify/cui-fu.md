---
doc_id: doc_integrations_dian_zi_shang_wu_shopify_cui_fu
language: zh-CN
title: "催付"
slug: cui-fu
path: integrations/dian-zi-shang-wu/shopify/cui-fu
document_group: integrations
path_in_group: dian-zi-shang-wu/shopify/cui-fu
parent_id: doc_integrations_dian_zi_shang_wu_shopify
order: 10
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T11:15:15.607Z
updated_at: 2026-04-02T11:15:15.607Z
last_synced_at: 2026-04-02T11:15:15.607Z
tags:
---

# 催付

通过WhatsApp对未支付的订单进行催付，帮助店铺提高收入。

## 开启催付

### 步骤1： 访问[Shopify Journey](https://www.ycloud.com/console/#/app/integrations/shopify/shopifyJourney)

<figure><img src="../../../.gitbook/assets/image (25).png" alt=""><figcaption></figcaption></figure>

### 步骤2：设置Sender

1. Sender：发送的商业号码
2. Template：发送的模板。若模板中有变量，建议使用Shopify变量
3. Send after：放弃支付多久之后进行触发。支持设置10分钟\~24小时后发送。
4. 默认过滤已经支付的订单。

<figure><img src="../../../.gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure>

### 步骤3：保存

点击保存按钮



### 步骤4：开启

<figure><img src="../../../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

## 查看数据

点击Logs进入触发记录页面，查看催付效果。

<figure><img src="../../../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>
