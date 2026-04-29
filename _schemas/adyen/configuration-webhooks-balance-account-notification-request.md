---
description: BalanceAccountNotificationRequest schema from Adyen API
layout: schema
name: BalanceAccountNotificationRequest
properties_list:
- description: Contains event details.
  name: data
  type: object
- description: 'The environment from which the webhook originated. Possible values: **test**, **live**.'
  name: environment
  type: string
- description: Type of webhook.
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-webhooks-balance-account-notification-request-schema.json
slug: configuration-webhooks-balance-account-notification-request
source_filename: configuration-webhooks-balance-account-notification-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-balance-account-notification-request-schema.json\",\n  \"title\": \"BalanceAccountNotificationRequest\",\n  \"description\": \"BalanceAccountNotificationRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"description\": \"Contains event details.\",\n      \"$ref\": \"#/components/schemas/BalanceAccountNotificationData\"\n    },\n    \"environment\": {\n      \"description\": \"The environment from which the webhook originated.\\n\\nPossible values: **test**, **live**.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"Type of webhook.\",\n      \"enum\": [\n        \"balancePlatform.balanceAccount.updated\",\n        \"balancePlatform.balanceAccount.created\"\n      ],\n      \"type\": \"string\"\n    }\n \
  \ },\n  \"required\": [\n    \"environment\",\n    \"type\",\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-balance-account-notification-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BalanceAccountNotificationRequest
---
