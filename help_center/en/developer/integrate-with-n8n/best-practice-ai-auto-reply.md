---
hidden: true
---

# Best Practice: AI Auto-Reply

This example will demonstrate how to implement a basic automated response workflow using n8n + large language models:

Upon receiving an inbound message, YCloud triggers an n8n workflow via a webhook, invokes a large language model to generate a response, and returns the message to the user through the YCloud API.

> YCloud Chatbot has built a comprehensive AI workflow for you, providing a fully integrated, straightforward AI knowledge base, corpora, and automated processes. You may click [this link ](/broken/pages/bJV1L3TuAvr6q0yPEQXi)to view details.

## Overall

<figure><img src="../../.gitbook/assets/image (822).png" alt=""><figcaption></figcaption></figure>

## Webhook Event

When configuring the Webhook event, please set the HTTP Method to POST, the Response to Immediate Return, and the Response Status Code to 200.

{% hint style="info" %}
Please take care to safeguard your Webhook URL and ensure that only a status code 200 is returned.
{% endhint %}

<figure><img src="../../.gitbook/assets/CleanShot 2025-12-24 at 14.19.49.png" alt=""><figcaption></figcaption></figure>

You must select WhatsApp.inbound\_message.received within the YCloud Webhook event. Upon triggering the YCloud Webhook, the n8n Webhook node will receive the complete inbound\_message data and automatically parse it into usable fields. As illustrated below:

<figure><img src="../../.gitbook/assets/image (823).png" alt=""><figcaption></figcaption></figure>

These fields will serve as input data for subsequent nodes (such as Data Table, AI Agent, HTTP Request, etc.) and may be referenced via Expression.

***

## Data Table

#### Data Table Design

#### Insert Row

This node is used to write data received via webhooks into a data table for subsequent querying or status management.

* Supports manual matching or automatic matching.
* Automatic matching requires field names to be identical.
* You may drag fields directly from the Input panel into configuration items, and n8n will automatically generate the Expression.

<figure><img src="../../.gitbook/assets/image (824).png" alt=""><figcaption></figcaption></figure>

#### Get Row

This node is used to read existing data from the Data Table. The condition can be defind as you want. At this best practice, we use wamid as the matching condition.

<figure><img src="../../.gitbook/assets/image (825).png" alt=""><figcaption></figcaption></figure>

Within this node, it is typically necessary to configure matching conditions (Condition).

This method is commonly used to determine whether a message has been processed or to retrieve historical context.

## AI Agent

### 1. Model Config

Before utilising the AI Agent, please configure the corresponding model information (such as OpenRouter, Ollama, etc.) within Credentials. This section will employ OpenRouter for configuration.

Screenshots of Credential configuration are omitted here; simply utilise the relevant APIs provided by OpenRouter. You may select your preferred model and return format; for this best practice example, choose grok-3 with TXT format.

<figure><img src="../../.gitbook/assets/CleanShot 2025-12-24 at 14.32.35.png" alt=""><figcaption></figcaption></figure>

### 2. AI Agent Node

Within the AI Agent node:

* Compose the prompt
* Utilise expressions to reference fields from webhooks or data tables as input. You may compose your desired prompt here; no additions are required. The prompt content may be freely customised according to business requirements.

<figure><img src="../../.gitbook/assets/image (827).png" alt=""><figcaption></figcaption></figure>

You may select different tools to connect to the AI Agent node; simply link them to the node.

<figure><img src="../../.gitbook/assets/CleanShot 2025-12-24 at 16.36.50.png" alt=""><figcaption></figcaption></figure>

> Note: The AI Agent supports an extended memory mechanism (Memory), enabling context management through databases or other storage methods.

Here you may view the final output information from the model.

<figure><img src="../../.gitbook/assets/image (829).png" alt=""><figcaption></figcaption></figure>

## Merge

The Merge node is used to combine the output data from multiple nodes, preparing it for subsequent API requests.

<figure><img src="../../.gitbook/assets/image (830).png" alt=""><figcaption></figcaption></figure>

Common patterns include:

* Append
* Combine
* Merge by Index

In the current example, the merge pattern is employed to concatenate multiple outputs into a single data structure for use by the HTTP Request node.

***

### HTTP Request

Finally, invoke the YCloud message sending interface via the HTTP Request node.

<figure><img src="../../.gitbook/assets/image (50).png" alt=""><figcaption></figcaption></figure>

* You may utilise the cURL examples provided in the YCloud [API documentation](https://docs.ycloud.com) for rapid configuration, inserting your API key into the location corresponding to X-API-KEY.
* Drag the merged field from the previous step into the request body.

{% hint style="warning" %}
Please note that the sender and recipient roles are **reversed** here, as this constitutes a reply message.
{% endhint %}

* Use Expression to dynamically populate message content, recipients, and other parameters.

At this point, a complete n8n workflow comprising Webhook → Large Language Model → Automated Response has been configured.

***

## Summary

By following the steps above, you can swiftly build an automated reply workflow using n8n to achieve:

* Webhook Listening
* Message Data Processing
* LLM Automated Content Generation
* Responding to Users via YCloud API

This example serves as a starting point for integration via n8n.



