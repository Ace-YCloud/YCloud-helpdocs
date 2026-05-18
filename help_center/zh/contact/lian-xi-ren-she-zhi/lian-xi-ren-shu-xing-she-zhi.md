# 联系人属性设置

联系人属性用于记录联系人基础资料、来源、标签和互动状态。通过联系人属性，你可以在联系人列表和联系人详情中查看客户信息，也可以基于属性进行筛选、分组和后续运营。



联系人属性包括**系统属性**和**自定义属性**：

* 系统属性：由 YCloud 自动生成或更新，例如昵称、手机号、来源、创建时间、最后联系时间等。
* 自定义属性：由成员根据业务需要手动创建，例如客户等级、购买意向、所属门店、业务类型等。

### 常见系统属性

常见联系人属性包括：

<table><thead><tr><th width="142.125">属性</th><th width="147.109375">英文字段</th><th width="66.94140625">类型</th><th>说明</th></tr></thead><tbody><tr><td>昵称</td><td>Nickname</td><td>文本</td><td>联系人的原始昵称，通常来自 WhatsApp 资料同步。</td></tr><tr><td>手机号</td><td>Phone number</td><td>文本</td><td>联系人的主要手机号，通常来自 WhatsApp 同步或手动录入。</td></tr><tr><td>邮箱</td><td>Email</td><td>文本</td><td>联系人的邮箱地址。</td></tr><tr><td>国家 / 地区</td><td>Country</td><td>文本</td><td>联系人所属国家或地区，通常根据手机号或资料信息识别。</td></tr><tr><td>来源</td><td>Source</td><td>文本</td><td>联系人来源，用于说明联系人是否来自消息、链接、导入、API、广告或其他入口。</td></tr><tr><td>来源 ID</td><td>Source ID</td><td>文本</td><td>联系人来源对应的唯一标识，通常用于记录原始广告来源或渠道来源。</td></tr><tr><td>来源 URL</td><td>Source URL</td><td>文本</td><td>联系人来源对应的原始 URL，例如广告、活动或入口链接。</td></tr><tr><td>标签</td><td>Tag</td><td>数组</td><td>分配给联系人的标签，可用于分类、筛选和后续运营。</td></tr><tr><td>负责人</td><td>Owner</td><td>文本</td><td>负责管理该联系人的成员邮箱。</td></tr><tr><td>创建时间</td><td>Create time</td><td>时间</td><td>联系人在系统中首次创建的时间。</td></tr><tr><td>最后联系时间</td><td>Last contacted</td><td>时间</td><td>最近一次与该联系人发生互动的时间。</td></tr><tr><td>最后联系的号码</td><td>Last connected number</td><td>文本</td><td>最近一次与该联系人沟通时使用的 WhatsApp Business 号码或渠道号码。</td></tr></tbody></table>

{% hint style="info" %}
带有 System 标记的属性为系统属性，通常由 YCloud 根据联系人资料、来源、会话、导入或集成数据自动生成或更新。
{% endhint %}

#### 来源

来源（Source / Contact source）是联系人最常用的系统属性之一。它表示联系人最初进入 YCloud 的来源，适合用于判断获客渠道、分析广告效果，或筛选不同入口进入的客户。

来源可能包含以下枚举值：

| 来源                    | 英文枚举值                 | 含义                           |
| --------------------- | --------------------- | ---------------------------- |
| 入站消息                  | Inbound message       | 联系人通过主动发送消息进入。               |
| 链接 / 二维码              | Link/QR Code          | 联系人通过链接或二维码进入。               |
| 手动添加                  | Manually added        | 联系人由成员手动添加。                  |
| 文件导入                  | File import           | 联系人通过文件批量导入。                 |
| Shopify               | Shopify               | 联系人来自 Shopify 集成。            |
| API 添加                | API added             | 联系人通过 API 创建。                |
| 广告                    | AD                    | 联系人来自广告相关入口。                 |
| TikTok 广告             | Tiktok AD             | 联系人来自 TikTok 广告。             |
| 帖子                    | Post                  | 联系人来自帖子相关入口。                 |
| 通话                    | Calling               | 联系人来自通话相关入口。                 |
| WhatsApp Business App | Whatsapp Business App | 联系人来自 WhatsApp Business App。 |
| 未知                    | Unknown               | 系统无法识别来源，或历史数据中没有记录来源。       |

例如，

当你想查看 TikTok 广告带来的联系人时，可以筛选“TikTok 广告”。当你想查看通过 Shopify 同步或创建的联系人时，可以筛选“Shopify”。

<figure><img src="../../.gitbook/assets/image (920).png" alt=""><figcaption></figcaption></figure>

### 新增自定义属性

如果系统属性不能满足你的业务管理需求，你可以新增自定义属性。

1. 登录 [YCloud 账号](https://www.ycloud.com)。
2. 导航至 **Contact > Settings > Attributes**。
3. 点击 **Add Attribute**。
4. 填写属性名称，并选择属性类型。
5. 点击 **Add** 完成添加。



### 编辑或删除属性

属性添加成功后，你可以在 **Contact > Settings > Attributes** 页面查看该属性，也可以根据需要进行编辑或删除。

编辑或删除属性前，建议确认该属性是否正在用于联系人筛选、分组、自动化流程或其他运营场景，避免影响已有联系人管理流程。



#### 步骤1、进入属性管理页

登录[YCloud账号](https://www.ycloud.com/console/#/entry/login)，导航至Contact > Settings > Attributes

<figure><img src="../../.gitbook/assets/image (363).png" alt=""><figcaption></figcaption></figure>

#### 步骤2、填写属性信息并提交

点击Add Attribute新增属性，点击Add完成添加

<figure><img src="../../.gitbook/assets/image (364).png" alt=""><figcaption></figcaption></figure>

#### 步骤3、查看新建的属性

添加成功可在后台查看；也可进行编辑或者删除操作

<figure><img src="../../.gitbook/assets/image (366).png" alt=""><figcaption></figcaption></figure>
