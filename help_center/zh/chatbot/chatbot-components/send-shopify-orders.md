# Send Shopify orders

当客户来询问Shopify订单详情时，可自动搜索客户在Shopify店铺中的订单，并回复订单信息。

{% hint style="info" %}
在使用该组件前，需要在Shopify店铺中安装[YCloud应用](https://apps.shopify.com/ycloud-whatsapp-sms)
{% endhint %}

## 最佳实践

1. 用自然语言识别的触发器识别用户意图，并确认客户是否是想查询Shopify的订单。
2. 当用户确认意图后，通过客户的手机号码自动查询其名下的订单信息，并组装信息后返回。
3. 若通过客户的手机号码未查询到订单，则使用 [Ask question](ask-a-question.md) 组件询问客户的订单号。
4. 询问到客户的订单号后，通过该信息继续查看Shopify的订单并反馈给客户。
5. 查询失败时，及时通过[Agent takeover](agent-takeover.md) 组件将到客户转人工进行对接。

<figure><img src="../../.gitbook/assets/image (931).png" alt=""><figcaption></figcaption></figure>

## 组件设置项

<figure><img src="../../.gitbook/assets/image (125).png" alt=""><figcaption></figcaption></figure>

### 搜索方式：

1. 通过客户的WhatsApp号码直接搜索。系统自动根据客户WhatsApp的号码搜索Shopify订单。
2. 根据客户提供的 Order ID进行搜索。前置条件是需要通过Ask question组件询问到订单号，并将其保存为“订单号”字段。



### 发送订单数量

当客户在Shopify搜索到多个订单时，可设置返回多少个订单数据。

支持设置的数值1\~50



### 发送的订单详情

您可以自由组装发送的订单信息，可通过插入“Shopify fields”来插入订单的数据。支持的订单数据有：

1. order\_id
2. order\_status
3. order\_link
4. item\_number
5. order\_amount
6. product\_name
7. shop\_name
8. total\_discounts
9. tracking\_url
10. tracking\_company
11. tracking\_id
12. currency



<br>

\
\
<br>

