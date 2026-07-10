---
doc_id: doc_shop_product
language: zh-CN
title: "商品管理"
slug: product
path: shop/product
document_group: shop
path_in_group: product
parent_id: doc_shop
order: 790
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

# 商品管理

{% hint style="info" %}
在尝试添加商品前，请先确认：您已成功创建店铺。[点此了解创建店铺](creatstore.md)
{% endhint %}



对商品进行管理，包含以下方面：

* 添加商品
* 商品预览、发布
* 商品归档、删除



## 添加商品

在Shop创建一个新的商品。

* 访问后台：Shop-Product
* 点击 Add new product，进入创建流程

<figure><img src="../.gitbook/assets/Shop_Product_CreatProduct.png" alt=""><figcaption><p>店铺后台-商品列表</p></figcaption></figure>

填写商品信息

<figure><img src="../.gitbook/assets/Shop_Product_Creat01.png" alt=""><figcaption><p>添加商品信息</p></figcaption></figure>

对于商品信息，我们将分为这几部分，分别介绍：

* [标题和描述](product.md#biao-ti-titile-miao-shu-description-xiang-guan)：使用富文本格式，创建有助于 “您的客户” 快速理解。
* [商品图片](product.md#shang-pin-tu-pian)：展示商品的主要图片信息。
* [价格和库存](product.md#jia-ge-yu-ku-cun)：设置基本价格、跟踪库存数量并管理多属性特定库存。
* [商品category分类](product.md#shang-pin-category)：定义商品是虚拟商品 or实物商品，会对履约和商品信息有一些影响。
* [商品类型](product.md#shang-pin-lei-xing)：catalog和广告相关的信息。





### 标题（Titile）、描述（Description）相关

{% hint style="warning" %}
您的客户会在商品详情介绍页、订单等位置，看到您填写的这些信息
{% endhint %}

<figure><img src="../.gitbook/assets/Shop_Product_Creat01-2.png" alt=""><figcaption><p>商品-添加/编辑商品-填写标题、描述</p></figcaption></figure>

**标题/Title**：您要向客户显示的产品名称。尽可能涵盖商品的所有关键信息（如用途、使用场景、关键词、属性规格等），方便用户快速了解。

**描述/Description**：填写关于产品的详细信息。此区域可使用富文本编辑器，因此您可以设置文本、图片、的格式，详细描述您的产品，以使您的潜在客户充分了解产品并向其进行营销。如果您是经销商，请勿使用制造商的确切描述，因为您需要让您的产品在搜索引擎中脱颖而出。



### 商品图片

{% hint style="warning" %}
您的客户会在商品详情介绍页、订单等位置，看到您填写的这些信息
{% endhint %}

<figure><img src="../.gitbook/assets/Shop_Product_Creat01-image.png" alt=""><figcaption><p>商品-添加/更新商品-图片image</p></figcaption></figure>

商品图片

* 点击upload选择图片上传；上传后，将在商品详情页进行展示。
* 图片的使用，有一些限制：
  * 图片大小 < 1Mb&#x20;
  * 宽高比1：1，如：400x400 px。
  * 支持的格式：jpg、jpeg、png
  * 最多可上传商品图片数量：10。（当上传达到10张照片后，只能删除旧照片再替换为新照片）

如果您需要了解图片的最终展示效果，可了解 [预览](product.md#shang-pin-yu-lan)。



### 价格与库存

{% hint style="info" %}
关于商品价格的币种，在创建店铺时已设置，[点此了解更多](creatstore.md)。
{% endhint %}

原价：市场上同类型产品的参考价格，是大家常说的市场价、划线价。仅作为参考，不参与实际的交易；

售价：商品的真实售卖价格。



#### 商品只有一个规格时

当商品只有一个sku 时，

只填写库存、市场价、售价，即可发布售卖。

<figure><img src="../.gitbook/assets/Shop_Product_creat01_spu.png" alt=""><figcaption><p>product-create-spu</p></figcaption></figure>



#### 商品有多个sku规格时

当商品有多个sku时，

点击后切换并添加多个sku

<figure><img src="../.gitbook/assets/Shop_Product_Creat01-SKU01.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Shop_Product_Creat01-SKU02.png" alt=""><figcaption></figcaption></figure>

1. 填写sku的变体规格信息：规格名称、售价、库存等，保证准确。



{% hint style="info" %}
注意 sku的availability，

* 当sku的availiablity = 打开状态，sku才是可售卖的。
* 当sku的availiablity = 关闭状态，sku无法被看见，也无法下单。
{% endhint %}



### 商品category

根据您发布的商品，是实物商品、还是虚拟商品，来进行选择。

* 实物商品：代表顾客购买后，该商品需要通过物流进行发货配送。
* 虚拟商品：代表顾客购买后，该商品不需要发货（如购买会员卡、电影播放许可）。

{% hint style="info" %}
根据你选择的类型，会决定 发货和运费的相关设置（见下图），是否必填。

请按需选择。
{% endhint %}

<figure><img src="../.gitbook/assets/Shop_Product_Creat01-spu-shipping.png" alt=""><figcaption></figcaption></figure>



### 商品类型

当您需要使用meta、Google的catalog开展广告时，需要注意这个选项。

选项包含3个，请按需选择：

* 全新商品
* 翻新商品
* 二手商品

{% hint style="info" %}
该选项为meta等catalog场景必须同步的商品信息，请务必填写准确。
{% endhint %}





## 商品预览、发布

当商品开始售卖时，您需要将该商品发布。 发布后的商品，才可以被消费者看到。

{% hint style="info" %}
正式发布前，建议您按如下步骤操作：

1. [预览商品](product.md#ku-cun)，再次检查所有信息。
2. [发布商品](product.md#shang-pin-zhuang-tai-yu-fa-bu)，将商品上架，再分享链接给顾客。
{% endhint %}



### 商品预览

想要了解商品的展示效果，可使用预览功能。

点击会打开该商品的详情页链接，您可以查看所有信息。

操作路径：

<figure><img src="../.gitbook/assets/Shop_product_preview.png" alt=""><figcaption></figcaption></figure>



### 商品状态与发布

&#x20;商品总共2个状态

* 非活跃：草稿，顾客看不到这个商品，也无法购买。
* 活跃：可售卖状态。顾客可以访问这个商品链接，并下单。

#### 商品发布

创建一个商品，保存后，默认状态为 ：非活跃（inactive） 。

<table><thead><tr><th width="159.59765625">商品状态</th><th width="142.265625">可执行的操作</th><th>执行操作后，发生的变化</th></tr></thead><tbody><tr><td>非活跃（inactive）</td><td>发布/publish<br><img src="../.gitbook/assets/Shop_product_publish (1).png" alt=""></td><td>点击publish，商品状态 : 活跃（active）</td></tr><tr><td>活跃（active）</td><td>下架/unpublish<br><img src="../.gitbook/assets/Shop_product_Unpublish.png" alt="" data-size="original"></td><td>点击unpublish，商品状态 : 非活跃（inactive）</td></tr><tr><td>所有状态</td><td><ul><li>edit</li><li>delete</li><li>archive</li></ul></td><td><ul><li>edit：编辑商品；</li><li>delete：删除商品；</li><li>archive：归档商品；</li></ul></td></tr></tbody></table>

点击上架商品

<figure><img src="../.gitbook/assets/Shop_product_publish (3).png" alt=""><figcaption><p>Shop-products-publish</p></figcaption></figure>

当发现商品的状态=已发布时，说明该商品已发布成功；



#### 商品下架

{% hint style="info" %}
在商品发布后，如果不打算继续售卖，可将商品下架。

下架后，您的客户无法浏览该商品、也无法下单；
{% endhint %}



当发现商品的状态=已发布时，可对该商品下架。

操作按下图：

<figure><img src="../.gitbook/assets/Shop_product_Unpublish (2).png" alt=""><figcaption></figcaption></figure>



#### WhatsApp内分享链接

商品发布后，通过whatsapp，可以吸引顾客来浏览商品并下单。

demo参考：

<table><thead><tr><th width="177.82421875">实际场景</th><th>展示demo1</th><th>demo2</th></tr></thead><tbody><tr><td>在WhatsApp内，将商品/订单link发给顾客</td><td><img src="../.gitbook/assets/Shop_inbox_chat_menu_sendProduct (2).png" alt=""></td><td>-</td></tr><tr><td>顾客浏览商品</td><td><img src="../.gitbook/assets/Shop_inbox_chat_product.jpeg" alt=""></td><td><img src="../.gitbook/assets/Shop_c_productpage01 (1).png" alt=""></td></tr><tr><td>顾客购买</td><td><img src="../.gitbook/assets/Shop_c_productpage02 (1).png" alt=""></td><td><img src="../.gitbook/assets/Shop_c_orderpage01 (2).jpeg" alt=""></td></tr></tbody></table>



## 商品归档、删除

如果你不再售卖某个商品，可以将其 归档 或删除。

* 删除：删除后，该商品不存在。您也无法再恢复此商品。
* 归档：将商品暂时标记为一个特殊状态。但你仍可以管理该商品，后续可恢复；



两者差异对比：

<table><thead><tr><th width="96.71484375">商品的操作</th><th width="121.875">商品状态</th><th width="125.19921875">是否能重新发布</th><th>Shop商品列表</th><th width="205.1953125">您的客户（消费者）是否可见</th></tr></thead><tbody><tr><td>删除</td><td>已删除</td><td>否</td><td><p>商品不可见、</p><p>商品不可操作</p></td><td>商品不可见</td></tr><tr><td>归档</td><td>归档/archive</td><td>是</td><td><p>商品可见、</p><p>商品可操作</p></td><td>商品不可见</td></tr></tbody></table>











