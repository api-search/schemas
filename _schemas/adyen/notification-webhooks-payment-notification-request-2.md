---
description: PaymentNotificationRequest-2 schema from Adyen API
layout: schema
name: PaymentNotificationRequest-2
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
schema_file: json-schema/notification-webhooks-payment-notification-request-2-schema.json
slug: notification-webhooks-payment-notification-request-2
source_filename: notification-webhooks-payment-notification-request-2-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-payment-notification-request-2-schema.json\",\n  \"title\": \"PaymentNotificationRequest-2\",\n  \"description\": \"PaymentNotificationRequest-2 schema from Adyen API\",\n  \"properties\": {\n    \"data\": {\n      \"description\": \"Contains event details.\",\n      \"$ref\": \"#/components/schemas/PaymentNotificationData\"\n    },\n    \"environment\": {\n      \"description\": \"The environment from which the webhook originated.\\n\\nPossible values: **test**, **live**.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"Type of notification.\",\n      \"enum\": [\n        \"balancePlatform.payment.created\",\n        \"balancePlatform.payment.updated\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"environment\",\n    \"type\"\
  ,\n    \"data\"\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-payment-notification-request-2-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentNotificationRequest-2
---
