# Message status rule

判断模板发送状态的组件，支持已读和回复状态的判断。用于对接收到消息后，做出不同反应的客户进行分流。

场景举例：发送了一条欢迎消息，对于回复了消息的客户，我们自动发送一条促活消息。对于收到消息没有回复的在不再打扰。



## Message status rule的设置项：

**判断的模板**：选需要判断状态的模板。

**等待的时间：**&#x5728;设置的时间内会进行模板消息状态的判断。

**后续连接节点：**

1. 在等待的时间内，满足了选择的状态时。
2. 在等待时间结束后，还未满足选择的状态时。

<figure><img src="../../.gitbook/assets/image (737).png" alt=""><figcaption></figcaption></figure>



## 添加方式

### 方式1：在Send template后直接连接。

将鼠标移动到Send template的连接节点上时，会出现两个快捷选项，分别是判断这条消息已读时或者回复时。点击后会自动连接一个新的Message statues rule组件。

<figure><img src="../../.gitbook/assets/image (732).png" alt=""><figcaption></figcaption></figure>



### 方式2：手动添加组件

手动添加的Message status rule是不会自动配置模板并连接。您需要在设置页面中手动选择模板和需要判断的状态。选择模板时，只能选择当前Journey中所有Send template已经选择了的模板。模板选择后，需要手动连接前置流程。

<figure><img src="../../.gitbook/assets/image (733).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (738).png" alt=""><figcaption></figcaption></figure>
