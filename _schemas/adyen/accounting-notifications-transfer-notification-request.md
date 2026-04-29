---
description: TransferNotificationRequest schema from Adyen API
layout: schema
name: TransferNotificationRequest
properties_list:
- description: Contains details about the event.
  name: data
  type: object
- description: 'The environment from which the webhook originated. Possible values: **test**, **live**.'
  name: environment
  type: string
- description: The type of the notification.
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounting-notifications-transfer-notification-request-schema.json
slug: accounting-notifications-transfer-notification-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounting-notifications-transfer-notification-request-schema.json\",\n  \"title\": \"TransferNotificationRequest\",\n  \"description\": \"TransferNotificationRequest schema from Adyen API\",\n  \"properties\": {\n    \"data\": {\n      \"description\": \"Contains details about the event.\",\n      \"$ref\": \"#/components/schemas/TransferNotificationData\"\n    },\n    \"environment\": {\n      \"description\": \"The environment from which the webhook originated.\\n\\nPossible values: **test**, **live**.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The type of the notification.\",\n      \"enum\": [\n        \"balancePlatform.transfer.created\",\n        \"balancePlatform.transfer.updated\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"environment\"\
  ,\n    \"data\"\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounting-notifications-transfer-notification-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransferNotificationRequest
---
