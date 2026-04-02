---
doc_id: doc_shop_orders_shipping_import
language: zh-CN
title: "物流信息批量导入"
slug: shipping-import
path: shop/orders/shipping-import
document_group: shop
path_in_group: orders/shipping-import
parent_id: doc_shop_orders
order: 0
status: published
translation_status: source
source_system: gitbook
source_external_id: 
source_revision: 
created_at: 2026-04-02T07:24:10.956Z
updated_at: 2026-04-02T07:24:10.956Z
last_synced_at: 2026-04-02T07:24:10.956Z
tags:
---

# 物流信息批量导入

### 能做什么

* 本功能仅针对您店铺内已存在的订单，用于更新发货状态与物流快递信息。**不会为店铺创建新的订单！**
* 更新内容包括：发货状态、承运商、运单号以及追踪链接。
* 对 **实物商品** 订单：导入成功后订单会被标记为 **已发货**，并向顾客展示物流信息。
* 对 **虚拟/数字商品** 订单：仅标记为 **已发货**（无需填写运单号或追踪链接）。

***

### 开始前准备

为确保履约流程顺畅，请先完成以下设置：

* 安装并创建店铺、添加商品、设置运费模板与支付方式（COD / PayPal）。
* 建议熟悉 **订单 → 发货 / 标记已付款（COD） / 退款与退货** 基本操作，[点此了解](./)。

***

### 下载模板

在 **Shop → 订单** 页面，点击 **导入**

&#x20;打开弹窗，再点击 **下载模板**。

**操作路径：**

<figure><img src="../../.gitbook/assets/shipping_info_entrance.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/shipping_info_template_entrance.png" alt=""><figcaption></figcaption></figure>



模板填写的注意事项‼️

### 快递导入模板的字段说明‼️

<table><thead><tr><th width="154.62109375">列名</th><th>说明</th><th>demo：实物订单</th><th>demo：虚拟商品</th></tr></thead><tbody><tr><td><code>Order_ID</code></td><td>系统生成的订单唯一标识，用于匹配目标订单。<strong>必填</strong></td><td>100001250814000155</td><td>100001250814000153</td></tr><tr><td><code>Shipping_Carrier</code></td><td>承运商名称,如 ：<br>SF、J&#x26;T、DHL 等<br><strong>实物商品：必填</strong><br><strong>虚拟商品：不填</strong></td><td>FedEx</td><td><strong>(不填，空着)</strong></td></tr><tr><td><code>Tracking_Number</code></td><td>运单号/追踪号。<br><strong>实物商品：必填</strong><br><strong>虚拟商品：不填</strong></td><td>1234 5678 9012</td><td><strong>(不填，空着)</strong></td></tr><tr><td><code>Tracking_Url</code></td><td>顾客点击“查看物流”使用的追踪链接。<br><strong>实物商品：必填</strong><br><strong>虚拟商品：不填</strong></td><td><a href="https://www.fedex.com/wtrk/track/?trknbr=123456789012">https://www.fedex.com/wtrk/track/?trknbr=123456789012</a></td><td><strong>(不填，空着)</strong></td></tr></tbody></table>





***

### 上传与处理

#### 1. 准备上传

点击 **上传**，进入文件选择器，

**操作路径：**

<figure><img src="../../.gitbook/assets/shipping_info_upload (1).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
&#x20;注意，请留意弹窗内，上传文件的要求：

* **csv**格式
* 最大 **15 MB**，**≤ 1,000** 行数据。
* 仅支持上传 **1 个文件/次**
{% endhint %}



***

#### 2. 选择文件，开始上传

选择一个csv文件，点击打开，

<figure><img src="../../.gitbook/assets/shipping_info_filepicker.png" alt=""><figcaption></figcaption></figure>

系统将自动开始解析表格

* 表格检测顺利通过后，就自动开始导入数据，并展示 执行结果（见4）
* 表格检测失败，则说明表格有问题，需要您根据问题检查文件（见3）



***

#### 3. 文件导入失败

如果您的表格 不符合导入的要求，系统将不会导入任何一条数据。

此时，您会收到一个具体的错误信息。需要您先调整文件。

**文件检测失败的截图demo**

<figure><img src="../../.gitbook/assets/shipping_info_error_csv.png" alt=""><figcaption></figcaption></figure>

具体失败原因，可查看[校验规则-文件级校验](shipping-import.md#wen-jian-ji-jiao-yan)



如果顺利通过检测，则开始导入csv的数据。

<figure><img src="../../.gitbook/assets/shipping_info_file_uploading.png" alt=""><figcaption></figcaption></figure>

注意，当文件内的数据行较多时，耗费时间也会相应增加，请耐心等待。



***

#### 4. 文件导入成功

<figure><img src="../../.gitbook/assets/shipping_info_result&#x26;reports.png" alt=""><figcaption></figcaption></figure>

执行导入结束，会展示导入的结果：

* 导入成功：x条
* 导入失败：y条

点击-**下载错误报告**

浏览器会下载导入失败的数据，并展示错误的原因。

点击 **下载失败行** 获取仅包含失败行的 CSV（格式说明如下）。

***

### 字段说明（模板列）

| 列名                 | 说明                                    |
| ------------------ | ------------------------------------- |
| `Order_ID`         | 系统生成的订单唯一标识，用于匹配目标订单。                 |
| `Shipping_Carrier` | 承运商名称（如 SF、J\&T、DHL 等）。               |
| `Tracking_Number`  | 运单号/追踪号。实物商品**必填**；数字商品忽略此字段。         |
| `Tracking_Url`     | 顾客点击“查看物流”使用的追踪链接。                    |
| import status      | 一般是失败                                 |
| error message      | <p>具体这条订单，导入失败的原因。<br>如：这笔订单id不存在</p> |

**示例内容：**

```csv
Order_ID,Shipping_Carrier,Tracking_Number,Tracking_Url
123456789012345678,FDX,123456789012,https://www.fedex.com/track
987654321000000001,,SF1234567890123,
```

> **Excel 小技巧**：
>
> 注意，当您用excel打开csv文件时，为避免长订单号被自动转为科学计数法或截断，建议将 `Order_ID` 列设置为“文本格式”，或在值前添加英文单引号 `'`。

***

### 校验与错误报告

系统将进行文件级与行级校验：

#### 文件级校验

* 表头缺失或不一致 → `Invalid template header`
* 非 CSV 类型 → `Unsupported file type`
* 文件为空或无有效行 → `No valid entries found`
* 文件超过大小或行数限制 → `Maximum allowed size is 15 MB and 1,000 rows`
* 上传多个文件 → `Please upload only one file at a time`

#### 行级校验

* `Order_ID` 为空、未找到或不属于当前店铺 → `Order not found`
* 同一 `Order_ID` 重复 → `Duplicate Order ID; skipped`
* 实物订单缺失或格式错误的 `Tracking_Number` → `Invalid Tracking Number`
* 数字商品订单跳过物流字段，仅标记为已发货

**失败行报告示例（CSV）：**

```csv
Order_ID,Shipping_Carrier,Tracking_Number,Tracking_Url,Result,Reason
412341234,,,,Failed,"Missing shipping data"
634563456354635,,,,Failed,"Order not found"
```

> 若遇网络或系统异常等提示，可能是网络波动引起的，请您几分钟后 再尝试导入。

***

### 常见问题

**Q1：订单已标记为“已发货”，还能更新物流信息吗？**\
可以，再次导入该 `Order_ID` 或手动编辑时，系统将使用最新信息进行覆盖。

**Q2：虚拟 / 数字商品需要填写运单号吗？**\
不需要，系统会自动标记为已发货，但不会保存任何物流信息。

**Q3：Shop 当前支持哪些支付方式？**\
为了便于订单履约流程理解，当前支持 **货到付款（COD）** 和 **PayPal 钱包**。

**Q4：Excel 把长订单号格式化成科学计数法（如 1.23E+17），怎么办？**\
请将该列设置为“文本格式”，或者在值前加英文单引号 `'` 进行规避。

**Q5：遇到出错行怎么处理？**\
系统会跳过这些行并生成失败行报告，标注问题原因。建议修正后重新上传。

**Q6：excel不小心操作，导致一条订单出现2条物流轨迹。**\
只要数据本身是有效的，系统就会执行。

如果您的excel出现2条一样的记录，那么会分别执行。

第一条记录：订单ID=001，订单变为已发货，物流轨迹/运营商等一并更新...

第二条记录：订单ID=001，订单已经是发货状态；覆盖更新物流运营商/物流单号等信息

