---
doc_id: doc_payments
language: zh-CN
title: "支付设置"
slug: payments
path: payments
document_group: 
path_in_group: payments
parent_id: 
order: 0
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T07:17:02.285Z
updated_at: 2026-04-02T07:17:02.285Z
last_synced_at: 2026-04-02T07:17:02.285Z
tags:
---

# 支付设置



{% hint style="info" %}
目前Shop支持的支付方式：

* 货到付款（Cash On Delivery，简称COD）
* Paypal 钱包
{% endhint %}



当您新开通shop时，所有支付方式都处于关闭状态，您可以按需激活。

<figure><img src="../.gitbook/assets/Shop_Shopbase_nopayment.png" alt=""><figcaption></figcaption></figure>

点击add，选择您需要的支付方式

<figure><img src="../.gitbook/assets/Shop_Shopbasic_payment_popup (1).png" alt=""><figcaption></figcaption></figure>

### 货到付款

1. 选择cash on delivery
2. 弹窗-点击Active

货到付款开通成功后，如下：

<figure><img src="../.gitbook/assets/Shop_Shopbasic_payment_cod(active).png" alt=""><figcaption></figcaption></figure>

*   此时，顾客在您的商店下单时，可以选择支付方式：货到付款

    * 当选择货到付款后，需要在 顾客未付款的情况下，由您先发货。顾客收到货后再决定是否确认收货、支付。



当您准备停止使用货到付款时，可以点击-Deactive：

<figure><img src="../.gitbook/assets/Shop_Shopbasic_Cod(deavtive-popup).png" alt=""><figcaption></figcaption></figure>

* Deactive确认后，该支付将被关闭。



### PayPal钱包

开启方式：

* 选择PayPal
* 点击active，
* 跳转到PayPal页面，需要您登录，并完成授权

<figure><img src="../.gitbook/assets/Payment_paypal_login.png" alt=""><figcaption></figcaption></figure>

* 输入您的PayPal商业账号：账号/密码- 登录
  * 注意，必须&#x662F;_**business account**_。个人账号无法绑定shop去收款。
* 确认授权-Ycloud Shop，完成
* 进入Shop后台并提示：绑定成功：

<figure><img src="../.gitbook/assets/paypal_oauth_successfully.png" alt=""><figcaption></figcaption></figure>

会自动跳转到payments模块，并展示绑定的PayPal企业账号：

<figure><img src="../.gitbook/assets/shop_Shopbase_paypal(active).png" alt=""><figcaption></figcaption></figure>

* PayPal激活后，顾客可以在下单时，选择使用PayPal钱包进行支付。



如您想停用PayPal支付，点击【deactivate】-【deactivate】，即可隐藏顾客购买流程中的PayPal钱包选项。

