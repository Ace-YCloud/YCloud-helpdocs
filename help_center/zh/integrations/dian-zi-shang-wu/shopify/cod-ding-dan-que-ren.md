# COD 订单确认

当Shopify店铺中产生了COD订单，自动发送一条WhatsApp的确认消息给买家。消息中包含确认按钮，当客户点击确认按钮后，把该COD订单自动标记为“已确认”。



## 活动设置

### 步骤1： 访问[Shopify Journey](https://www.ycloud.com/console/#/app/integrations/shopify/shopifyJourney)

点击编辑

<figure><img src="../../../.gitbook/assets/image (695).png" alt=""><figcaption></figcaption></figure>

### 步骤2：编辑内容

#### 步骤2.1 选择Sender

选择一个发送的WhatsApp账号。注意，需要发送的模板必须在这个号码归属的WABA下。

<figure><img src="../../../.gitbook/assets/image (696).png" alt=""><figcaption></figcaption></figure>

#### 步骤2.2 选择Template

选择要发送的模板

<figure><img src="../../../.gitbook/assets/image (697).png" alt=""><figcaption></figcaption></figure>

若模板中有变量，可选择shopify中的变量进行替换。

<figure><img src="../../../.gitbook/assets/image (699).png" alt=""><figcaption></figcaption></figure>

#### 步骤2.3 选择“确认”按钮。

当用户点击该按钮时，YCloud将会给Shopify 的订单打上“已确认” 即 Confirmed 的标签。

<figure><img src="../../../.gitbook/assets/image (700).png" alt=""><figcaption></figcaption></figure>

#### 步骤2.4 选择“取消”按钮

当用户点击该按钮时，YCloud将会给Shopify 的订单打上“已取消” 即 Canceled 的标签。

<figure><img src="../../../.gitbook/assets/image (701).png" alt=""><figcaption></figcaption></figure>



#### 步骤2.5 设置发送时间

下单后多久触发这条确认信息

<figure><img src="../../../.gitbook/assets/image (702).png" alt=""><figcaption></figcaption></figure>

#### 2.6 设置追踪时间

超过追踪时间后，客户不可再确认改订单。

可选项：给未确认的订单打标为“未回复”即 Not reply。

<figure><img src="../../../.gitbook/assets/image (705).png" alt=""><figcaption></figcaption></figure>



#### 步骤2.7 点击保存

确认无误后点击保存按钮。

<figure><img src="../../../.gitbook/assets/image (706).png" alt=""><figcaption></figcaption></figure>

### 步骤3：开启COD 订单确认

<figure><img src="../../../.gitbook/assets/image (708).png" alt=""><figcaption></figcaption></figure>

## 查看数据

点击Logs查看订单确认情况

<figure><img src="../../../.gitbook/assets/image (710).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (709).png" alt=""><figcaption></figcaption></figure>

可进入Shopify订单页面确认订单的Confirmed, Cancelled, Not reply 的标签
