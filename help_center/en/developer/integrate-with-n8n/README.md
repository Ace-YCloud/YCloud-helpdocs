# Integrate With n8n

## Introduction

YCloud supports automated integration via n8n.

n8n is an open-source visual workflow automation platform that enables flexible integration between YCloud Webhooks, API events, and third-party systems such as CRMs, databases, and AI services.

In typical use cases for YCloud, n8n is commonly employed for:

* Receive YCloud Webhook event.
* Conditional evaluation and processing of messages or user actions.
* Invoke external APIs for analysis.
* Synchronise results to CRM, internal systems or data warehouses.

## Preparation

Before proceeding, please ensure that the following conditions are met:

* Deployed and accessible n8n instances.
* The login credentials and permissions for n8n have been obtained.
* Should you require access to large language models or third-party APIs, please ensure you have the corresponding API keys prepared in advance.

## n8n Official Documentation

For information on installing n8n, its fundamental concepts, and usage methods, please refer directly to the official n8n documentation:

👉 [https://docs.n8n.io](https://docs.n8n.io/)

The following content is fully explained in the official documentation:

* Fundamental Concepts of Workflow and Node
* Configuration Methods for Webhook Triggers
* Expression Syntax
* Credentials Management
* Execution Records and Debugging Methods

## Integration methods with YCloud

Within YCloud, the Webhook address can be configured as n8n's Webhook URL, enabling n8n to act as an intermediary layer for event handling.

## Note

* n8n is a third-party tool; Please make sure using the verified node.
* It is recommended to distinguish between the test environment (Test URL) and the production environment (Production URL) within n8n.
* Please manage sensitive information such as API keys and webhook addresses with due care.
