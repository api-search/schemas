---
description: TransactionNotificationRequestV4 schema from Adyen API
layout: schema
name: TransactionNotificationRequestV4
properties_list:
- description: Contains details about the event.
  name: data
  type: object
- description: 'The environment from which the webhook originated. Possible values: **test**, **live**.'
  name: environment
  type: string
- description: Type of the webhook.
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transaction-webhooks-transaction-notification-request-v4-schema.json
slug: transaction-webhooks-transaction-notification-request-v4
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transaction-webhooks-transaction-notification-request-v4-schema.json\",\n  \"title\": \"TransactionNotificationRequestV4\",\n  \"description\": \"TransactionNotificationRequestV4 schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"description\": \"Contains details about the event.\",\n      \"$ref\": \"#/components/schemas/Transaction\"\n    },\n    \"environment\": {\n      \"description\": \"The environment from which the webhook originated.\\n\\nPossible values: **test**, **live**.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"Type of the webhook.\",\n      \"enum\": [\n        \"balancePlatform.transaction.created\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"environment\",\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transaction-webhooks-transaction-notification-request-v4-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransactionNotificationRequestV4
---
