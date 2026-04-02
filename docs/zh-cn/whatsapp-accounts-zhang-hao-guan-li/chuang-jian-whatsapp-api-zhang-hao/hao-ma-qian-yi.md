---
doc_id: doc_whatsapp_accounts_zhang_hao_guan_li_chuang_jian_whatsapp_api_zhang_hao_hao_ma_qian_yi
language: zh-CN
title: "号码迁移"
slug: hao-ma-qian-yi
path: whatsapp-accounts-zhang-hao-guan-li/chuang-jian-whatsapp-api-zhang-hao/hao-ma-qian-yi
document_group: whatsapp-accounts-zhang-hao-guan-li
path_in_group: chuang-jian-whatsapp-api-zhang-hao/hao-ma-qian-yi
parent_id: doc_whatsapp_accounts_zhang_hao_guan_li_chuang_jian_whatsapp_api_zhang_hao
order: 30
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T11:07:53.930Z
updated_at: 2026-04-02T11:07:53.930Z
last_synced_at: 2026-04-02T11:07:53.930Z
tags:
---

# 号码迁移

号码迁移是指在 WhatsApp 商业帐户 (WABA) 之间迁移其WhatsApp API 号码，并保留其显示名称、质量评级、模板消息限制、官方商业帐户状态以及已批准的高质量模板。

通常，只有当客户想要将其WhatsApp API号码从一个解决方案合作伙伴转移到另一个解决方案合作伙伴时，才会执行迁移。

_例如：您在使用YCloud之前就已经在其他服务商处注册了WhatsApp  API账号，这时您可以考虑将号码迁移到YCloud上新创建的WABA中继续使用。_



## 迁移准备

1. YCloud账号中已经创建好WABA，且该WABA跟迁移的号码的WABA归属于同一个Business manager(BM)。若您还没有创建WABA，[请参考创建WABA教程](tong-guo-qian-ru-shi-zhu-ce-chuang-jian-waba.md)
2. 关掉迁移号码的两步验证。

## 迁移须知

1. 号码迁移只能在同一个BM，不同的WABA下进行迁移。
2. 迁移的号码必须已通过显示名称的审核，并且迁移时，名称不处于正在修改的过程中。
3. 号码的历史聊天记录不会迁移，请在原服务商处备份好记录。
4. 迁移后的号码质量、绿标、配置等号码属性不会发生变化。
5. 号码所属WABA下的所有已批准的高质量模板会同步过来，低质量或者不可用的模板均不能同步。迁移后，模板的质量评级会从头开始。

## 正式迁移

### 步骤1：关闭号码（需迁移的号码）的两步验证

登录BM后台，找到号码的管理页面，并关闭两步验证。具体步骤见下

提示：如果您原先的号码注册不是由您操作的，请联系注册人或者管理员进行关闭。

#### 步骤1.1：进入WABA管理页面

访问 [Business 管理页面](https://business.facebook.com/settings/whatsapp-business-accounts/)，登录过程中可能需要先登录此账号的管理员Facebook账号。

选择要迁移的号码的归属WABA > Settings > WhatsApp manager。

<figure><img src="../../.gitbook/assets/image (591).png" alt=""><figcaption><p>Business Manager settings</p></figcaption></figure>

####

#### 步骤1.3： 进入号码管理页面

点击导航栏的 Phone numbers，选择要迁移的号码，点击号码的设置图标。

<figure><img src="../../.gitbook/assets/image (115).png" alt=""><figcaption><p>WABA settings</p></figcaption></figure>

#### 步骤1.4：关闭号码的两步验证&#x20;

在号码管理页面中找到 Two-step verification，点击 Turn off two-step verification

<figure><img src="../../.gitbook/assets/image (117).png" alt=""><figcaption><p>Phone number settings</p></figcaption></figure>



### 步骤2：进行嵌入式注册

完成以上操作步骤后，即可进行号码迁移流程

#### 步骤2.1：登入YCloud开始迁移

访问[WhatsApp accounts](https://www.ycloud.com/console/#/app/dashboard/account)页面 ，点击 **添加号码**

<figure><img src="../../.gitbook/assets/image (167).png" alt=""><figcaption></figcaption></figure>

#### 步骤2.2：选择迁移号码

<figure><img src="../../.gitbook/assets/image (39).png" alt=""><figcaption></figcaption></figure>

#### 步骤2.3：确认迁移

<figure><img src="../../.gitbook/assets/image (40).png" alt=""><figcaption></figcaption></figure>

#### 步骤2.4：确认已关闭2fa

<figure><img src="../../.gitbook/assets/image (44).png" alt=""><figcaption></figcaption></figure>

#### 步骤2.5：输入需要迁移的号码

<figure><img src="../../.gitbook/assets/image (42).png" alt=""><figcaption></figcaption></figure>

#### 步骤2.6：输入验证码完成验证

Tip：中国大陆地区（+86）建议使用语音电话来接收验证码。

<figure><img src="../../.gitbook/assets/image (261).png" alt=""><figcaption></figcaption></figure>





#### 步骤2.7 绑定成功

弹窗关闭后YCloud会开始迁移您的号码，迁移成功后会显示在绑定的WABA中，且手机号码的状态为Connected。

若绑定失败可联系客服咨询。

