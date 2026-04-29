---
description: MerchantCreatedNotificationRequest schema from Adyen API
layout: schema
name: MerchantCreatedNotificationRequest
properties_list:
- description: Timestamp for when the webhook was created.
  name: createdAt
  type: string
- description: Contains event details.
  name: data
  type: object
- description: 'The environment from which the webhook originated. Possible values: **test**, **live**.'
  name: environment
  type: string
- description: Type of notification.
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-webhooks-merchant-created-notification-request-schema.json
slug: management-webhooks-merchant-created-notification-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-webhooks-merchant-created-notification-request-schema.json\",\n  \"title\": \"MerchantCreatedNotificationRequest\",\n  \"description\": \"MerchantCreatedNotificationRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"createdAt\": {\n      \"description\": \"Timestamp for when the webhook was created.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"data\": {\n      \"description\": \"Contains event details.\",\n      \"$ref\": \"#/components/schemas/AccountCreateNotificationData\"\n    },\n    \"environment\": {\n      \"description\": \"The environment from which the webhook originated.\\n\\nPossible values: **test**, **live**.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"Type of notification.\",\n \
  \     \"enum\": [\n        \"merchant.created\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"environment\",\n    \"createdAt\",\n    \"data\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-webhooks-merchant-created-notification-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: MerchantCreatedNotificationRequest
---
