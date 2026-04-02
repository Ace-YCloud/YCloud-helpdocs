---
doc_id: doc_contact_owner_gui_shu_she_zhi_zhuan_shu_ke_fu_xiao_shou_gui_shu
language: zh-CN
title: "Owner归属设置（专属客服/销售归属）"
slug: owner-gui-shu-she-zhi-zhuan-shu-ke-fu-xiao-shou-gui-shu
path: contact/owner-gui-shu-she-zhi-zhuan-shu-ke-fu-xiao-shou-gui-shu
document_group: contact
path_in_group: owner-gui-shu-she-zhi-zhuan-shu-ke-fu-xiao-shou-gui-shu
parent_id: doc_contact
order: 440
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T11:05:31.575Z
updated_at: 2026-04-02T11:05:31.575Z
last_synced_at: 2026-04-02T11:05:31.575Z
tags:
---

# Owner归属设置（专属客服/销售归属）

Owner是归属人的Email邮箱。在Contact中支持给每个客户设置1个Owner，这个Owner主要用于销售归属的判断。在YCloud的产品中，支持在Inbox(收件箱）收到消息时，根据客户归属进行对话分配。



## 如何设置Owner？

### 方法1: 在Contact中单个编辑

在Contact中找到客户的信息，点击后展开编辑页面。

<figure><img src="../.gitbook/assets/image (389).png" alt=""><figcaption></figcaption></figure>

找到Owner设置项，设置Owner。

输入Owner的email邮箱后点击保存，同时也支持下拉选择已存在的Agent（Inbox中的Agent）

<figure><img src="../.gitbook/assets/image (105).png" alt=""><figcaption></figcaption></figure>



### 方法2: 在Inbox中设置Owner

登录Inbox后，展开用户信息栏。点击Owner，选择想要转接的Owner，即刻完成转接。

<figure><img src="../.gitbook/assets/image (395).png" alt=""><figcaption></figcaption></figure>



### 方法3: 批量导入客户信息，并附带Owner

点击 Contact > Contact list > + New contacts > Upload a file

<figure><img src="../.gitbook/assets/image (396).png" alt=""><figcaption></figcaption></figure>

点击 【Download Template】 进行模板下载

<figure><img src="../.gitbook/assets/image (398).png" alt=""><figcaption></figcaption></figure>

编辑模板。保存后上传至YCloud。

<figure><img src="../.gitbook/assets/image (399).png" alt=""><figcaption></figcaption></figure>

上传完成后确认匹配字段无误，后点击【Next】

<figure><img src="../.gitbook/assets/image (400).png" alt=""><figcaption></figcaption></figure>

确认能够成功上传的数量，确认无误后点击 【Next】

<figure><img src="../.gitbook/assets/image (401).png" alt=""><figcaption></figcaption></figure>

完成上传

<figure><img src="../.gitbook/assets/image (402).png" alt=""><figcaption></figcaption></figure>



### 方法4: API上传

API文档：

* 点击查看[更新用户数据接口](https://docs.ycloud.com/reference/contact-update)
* 点击查看[新增用户数据接口](https://docs.ycloud.com/reference/contact-create)



Owner字段：OwnerEmail

非必填，需传入归属人的Email邮箱

<figure><img src="../.gitbook/assets/企业微信截图_9a00ba3e-a664-4962-a05c-df66026086be_副本.jpg" alt=""><figcaption></figcaption></figure>





