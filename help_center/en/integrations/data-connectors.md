---
description: Connect external databases and create fully automated customer interactions.
---

# Data connectors

## What are data connectors?

Data connectors are deeply embedded integration that can connect your live external data with us.&#x20;

A great way to get started is to think of those common questions that your teammates spend considerable time answering, using information currently not available in our platform.

These can be questions where your customers simply want to get information that you store on an external system such as, “Is my order delivered?”, or update information such as, "Reschedule a delivery" or "Process a refund" in your external system.

## Creating a data connector

First, navigate to Integrations > Data connectors

<figure><img src="../.gitbook/assets/image (760).png" alt=""><figcaption></figcaption></figure>

This is where you can set up data connectors to connect your external data. You can create one by clicking the \[+ New data connector] button. You can also search for specific data connectors by their name and status.

<figure><img src="../.gitbook/assets/image (761).png" alt=""><figcaption></figcaption></figure>

## Name and description

Give your data connector a name that clearly indicates its specific function (e.g., “retrieve\_order\_id”). In the description field, inform your teammates about when to use this connector and what data it will retrieve (e.g., “Fetches order details for a provided Order ID”).

<figure><img src="../.gitbook/assets/image (762).png" alt=""><figcaption></figcaption></figure>

## API connection

### **API request**

Next, fill in the request details. This is where you’ll need to enter the HTTPS URL to the 3rd party system you’re connecting to.

You can specify what data connector you’d like this request to take by selecting the method:

* **GET** - Read and store information from the 3rd party system.
* **POST** - Create or add information to the 3rd party system.
* **PUT** - Update information in the 3rd party system.
* **DELETE** - Remove information from the 3rd party system.
* **PATCH** - Update information in the 3rd party system.

<figure><img src="../.gitbook/assets/image (763).png" alt=""><figcaption></figcaption></figure>

### **HTTP headers**

You can choose to add any additional parameters to this request by clicking **Add header** and then add **Key value pair** under HTTP Headers:

<figure><img src="../.gitbook/assets/image (764).png" alt=""><figcaption></figcaption></figure>

### **Request body**

If you're making a POST or a PUT request, you'll have an option to provide a request body to include any data you want to send in the request:

<figure><img src="../.gitbook/assets/image (765).png" alt=""><figcaption></figcaption></figure>

### Test response

Next, you’ll need to test the response for this data connector to make sure it’s fetching the right data from the external system you’re connecting to.

{% hint style="warning" %}
**Important:** Testing this request makes a connection with the API so it will complete the data connector you have created. For example, if you’ve asked it to DELETE data from the API, this information will be deleted. Try testing with a GET request to ensure you’re only reading information and not changing it.
{% endhint %}

Click **Test request** to check the data connector has been configured correctly.

<figure><img src="../.gitbook/assets/image (766).png" alt=""><figcaption></figcaption></figure>

### Set live

Once you’ve tested your data connector successfully, you’re ready to set it live.

<figure><img src="../.gitbook/assets/image (767).png" alt=""><figcaption></figcaption></figure>

### Set to draft

If you want to deprecate old data connectors that are no longer required, you can move them into draft state.

You can either click on the data connector you want to move to draft, then select Set to draft or Turn off the status switch in the list.

<figure><img src="../.gitbook/assets/image (768).png" alt=""><figcaption></figcaption></figure>

This will check for any dependencies on this data connector. You'll need to review and resolve these dependencies before moving it to draft state.
