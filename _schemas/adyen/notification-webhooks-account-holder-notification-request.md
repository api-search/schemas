---
description: AccountHolderNotificationRequest schema from Adyen API
layout: schema
name: AccountHolderNotificationRequest
properties_list:
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
schema_file: json-schema/notification-webhooks-account-holder-notification-request-schema.json
slug: notification-webhooks-account-holder-notification-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-account-holder-notification-request-schema.json\",\n  \"title\": \"AccountHolderNotificationRequest\",\n  \"description\": \"AccountHolderNotificationRequest schema from Adyen API\",\n  \"properties\": {\n    \"data\": {\n      \"description\": \"Contains event details.\",\n      \"$ref\": \"#/components/schemas/AccountHolderNotificationData\"\n    },\n    \"environment\": {\n      \"description\": \"The environment from which the webhook originated.\\n\\nPossible values: **test**, **live**.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"Type of notification.\",\n      \"enum\": [\n        \"balancePlatform.accountHolder.updated\",\n        \"balancePlatform.accountHolder.created\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n   \
  \ \"environment\",\n    \"type\",\n    \"data\"\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-account-holder-notification-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AccountHolderNotificationRequest
---
