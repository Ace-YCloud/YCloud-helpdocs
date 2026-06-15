---
doc_id: doc_integrations_qu_dao_quan_qiu_duan_xin_duan_xin_gong_neng_qun_fa_xiao_xi
language: zh-CN
title: "群发消息"
slug: qun-fa-xiao-xi
path: integrations/qu-dao/quan-qiu-duan-xin/duan-xin-gong-neng/qun-fa-xiao-xi
document_group: integrations
path_in_group: qu-dao/quan-qiu-duan-xin/duan-xin-gong-neng/qun-fa-xiao-xi
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

# 群发消息

批量群发短信消息。

{% hint style="info" %}
注意：YCloud对所有群发的短信消息都会进行审核。部分国家地区的消息需要提前进行报备。有问题请联系客服处理。
{% endhint %}

## 步骤1：入口

登录YCloud并访问[Campaign](https://www.ycloud.com/console/#/app/bulkMessages/logs)



## 步骤2：创建SMS群发

点击创建按钮，选择SMS群发

<figure><img src="../../../../.gitbook/assets/image (686).png" alt=""><figcaption></figcaption></figure>

## 步骤3: 设置收件人

提供3种设置方式：

1. 手动输入手机号码
2. 上传手机号码的文件
3. 选择Contact中的人群

#### 手动输入手机号码

在多行文本字段中输入电话号码，每一行只能输入一个号码。请确保该号码采用国际格式，并应以国家/地区代码开头。例如，如果英国号码是 44，电话号码是 7759398257，那么您应该输入 +447759398257。 如果您已有 Excel 文件，则可以复制电话号码列并将其粘贴到框中。

<figure><img src="../../../../.gitbook/assets/image (687).png" alt=""><figcaption></figcaption></figure>

#### 上传手机号码文件

1. 下载模板，填写电话号码。
2. 打开模板文件，填写电话号码
   * 电话号码必须在第一栏，并命名为“phone”。
   * &#x20;如果消息中没有任何变量，则可以删除模板的其他列。
   * 如果消息中有变量，则可以从第二列第一行开始输入变量名称。\
     例如，短信是“_嗨#name#，您的余额低于#balance#_ ”。然后你可以设置一个名为“ _name_ ”的变量和一个名为“ _balance_ ”的变量

<figure><img src="../../../../.gitbook/assets/image (688).png" alt=""><figcaption></figcaption></figure>

#### 选择Contact中的人群

若您还未创建人群，可在Cotact中添加Segment。相关操作请查看[联系人分组](../../../../contact/lian-xi-ren-fen-zu.md)

<figure><img src="../../../../.gitbook/assets/image (689).png" alt=""><figcaption></figcaption></figure>



## 步骤4：设置群发信息

设置内容

* 群发活动的名称
* Signature/Sender ID：如果您在目标国家/地区有自己的发件人 ID，则会有一个发件人 ID 选择。Signature为发送中国大陆地区时的签名，若没有请联系客服获取支持。
* 信息内容：输入短信内容。请注意框内提示的字数和消息计费条数。
  * 变量：若通过文件上传手机号码，文件中有变量，可在编辑框上方中点击变量名称进行插入。
  * 选择历史模板：可点击 History按钮选择历史模板，历史审核通过模板无需二次审核
  * 短链接：支持将长链转为短链从而减少内容字数。
* 发送时间设置：立即发送和定时发送
* 活动审核通知：您可以设置一个自己的手机号码，群发活动审核通过后会进行短信提醒。

内容填写完成后，可点击下一步。<br>

<figure><img src="../../../../.gitbook/assets/image (690).png" alt=""><figcaption></figcaption></figure>

## 步骤5：确认信息

确认信息后点击 提交 按钮

<figure><img src="../../../../.gitbook/assets/image (692).png" alt=""><figcaption></figcaption></figure>

提交成功提示

<figure><img src="../../../../.gitbook/assets/image (693).png" alt=""><figcaption></figcaption></figure>

