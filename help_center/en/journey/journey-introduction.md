# Journey Introduction

Journey is an automation process that helps businesses trigger a series of actions based on customer behavior. You can use it to send messages to customers who have triggered an event, automatically tag them, and more.

Example:

In an e-commerce scenario, you can send notifications based on the customer's lifecycle, such as: subscription success notification, abandoned cart notification, order reminder, shipping reminder, order cancellation reminder, etc.

For an App company, you can use Journey to activate customers. For example, when a customer registers for the App, after waiting for N days, if the customer has not been activated, you can automatically send a message to promote activation.

## Understanding Journey Features:

### Components Included in Journey:

<table><thead><tr><th width="145">Component</th><th width="304">Function</th><th></th></tr></thead><tbody><tr><td>Trigger</td><td><p>Trigger is the core function of Journey, used to set the event and conditions that will trigger it.</p><p>Only users who meet all the conditions in the Trigger will activate the Journey.</p></td><td><img src="../.gitbook/assets/image (507).png" alt="" data-size="original"></td></tr><tr><td>Send template</td><td>Component for setting the content to be sent</td><td><img src="../.gitbook/assets/image (508).png" alt="" data-size="original"></td></tr><tr><td>Message status rule</td><td>Determines the status of the template message</td><td><img src="../.gitbook/assets/image (509).png" alt="" data-size="original"></td></tr><tr><td>Add tag</td><td>Tagging</td><td><img src="../.gitbook/assets/image (510).png" alt="" data-size="original"></td></tr><tr><td>Wait</td><td>Waiting</td><td><img src="../.gitbook/assets/image (511).png" alt="" data-size="original"></td></tr></tbody></table>

### Component Connection

Components need to be connected to each other, and they will be executed in the order of the connections.

<figure><img src="../.gitbook/assets/image (512).png" alt=""><figcaption></figcaption></figure>

### Setting Journey Goals and Exit Conditions

#### **Goals**:

Used to measure the effectiveness of Journey. You can set the statistics time, and continuously count whether the customer meets the goal conditions after being triggered. When the customer meets the conditions, the number of completed goals for Journey increases by one.

{% hint style="info" %}
Note: Goals are only for data statistics, and completing a goal does not mean the customer will exit Journey. Only by meeting the [**exit conditions**](journey-introduction.md#tui-chu-tiao-jian), or after executing the last component of Journey, will the customer exit.
{% endhint %}

#### **Exit Conditions**:

Once a user enters Journey, their compliance with exit conditions will be continuously assessed. If they meet the conditions, they will immediately exit, regardless of which stage they are in Journey, meaning they will no longer execute subsequent components.

<figure><img src="../.gitbook/assets/image (514).png" alt=""><figcaption></figcaption></figure>
