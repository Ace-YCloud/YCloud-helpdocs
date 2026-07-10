---
doc_id: doc_shop_shipping
language: zh-CN
title: "运费设置"
slug: shipping
path: shop/shipping
document_group: shop
path_in_group: shipping
parent_id: doc_shop
order: 770
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T11:18:00.934Z
updated_at: 2026-04-02T11:18:00.934Z
last_synced_at: 2026-04-02T11:18:00.934Z
tags:
---

# 运费设置

Shop支持3种运费模式：

1. 免运费：不收运费
2. 固定运费：设置一个固定的运费金额。每一笔订单，都按此价格 收取运费
3. 满x元免运费：当订单支付金额 >= {您设置的金额门槛}时，不收取运费。



## 设置运费模板

{% hint style="info" %}
在正式营业前，Shop需要配置好运费模板。避免因没收运费导致损失。
{% endhint %}

位置：Shop-Shop-Shipping

<figure><img src="../.gitbook/assets/Shop_Shopbasic_Shipping.png" alt=""><figcaption></figcaption></figure>

点击- 添加，

<figure><img src="../.gitbook/assets/Shop_Shopbasic_Shipping_add (1).png" alt=""><figcaption></figcaption></figure>

*   选择市场

    * 选择Global：Shop售卖到的所有国家，都采用同一个运费标准；
    * 选择目标销售市场：针对勾选的几个地区，将采用同一个运费标准。


* 运费计算方式，目前有3种
  * 免运费：针对选择的市场，有客户下单时，不收取运费。
  * 固定运费：设置一个固定的运费金额。针对选择的市场，客户每下一笔订单，都按此价格 收取运费。
  * 固定+免运费门槛：在您选择的市场范围中
    * 当订单支付金额 < {订单金额门槛}：按固定运费收取；
    * 当订单支付金额 > =  {订单金额门槛}：不收取运费。

{% hint style="info" %}
运费模板的设置，一定要包含{所有目标市场的国家} ，否则可能出现损失。

您的客户下单后，可能因为没设置运费，所以运费=0，导致您收入受损。
{% endhint %}

当出现上述问题时，系统会有提示文案，见下图：

<figure><img src="../.gitbook/assets/Shop_Shopbasic_Shipping_error01.png" alt=""><figcaption><p>Shop-Shipping-tips</p></figcaption></figure>

以上图为例，该文案说明：{美国、南非、中国台湾}国家，未设置运费规则。

* 此时，请按本篇指引，对提示国家 添加运费设置。



### 示例demo

提供一些常见的运费收取场景和配置的示例，便于理解。

<table><thead><tr><th width="237.78125">场景</th><th>配置规则</th></tr></thead><tbody><tr><td>全球市场,统一免运费</td><td><img src="../.gitbook/assets/Shop_Shopbasic_Shipping_add01.png" alt=""></td></tr><tr><td><p>全球市场，</p><p>统一收取固定运费9.9$</p></td><td><img src="../.gitbook/assets/Shop_Shopbasic_Shipping_add02.png" alt=""></td></tr><tr><td>全球市场，<br>满159$免运费<br>不满159$收9.9$</td><td><img src="../.gitbook/assets/Shop_Shopbasic_Shipping_add03.png" alt=""></td></tr><tr><td>收货地在美国，收取运费：20$<br>收货地在中国（内地+香港），收取运费：10$<br>收货地在其他国家，手运费9.9$；<br></td><td>1、美国配置<br><img src="../.gitbook/assets/Shop_Shopbasic_Shipping_add04.png" alt=""><br>2、中国<br><img src="../.gitbook/assets/Shop_Shopbasic_Shipping_add05.png" alt=""><br><br>3、其他国家<br><img src="../.gitbook/assets/Shop_Shopbasic_Shipping_add06.png" alt=""></td></tr></tbody></table>

添加完运费设置后，

可点此了解 [添加商品](product.md)
