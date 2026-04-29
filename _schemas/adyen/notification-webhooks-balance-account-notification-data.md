---
description: BalanceAccountNotificationData schema from Adyen API
layout: schema
name: BalanceAccountNotificationData
properties_list:
- description: ''
  name: balanceAccount
  type: object
- description: Unique identifier of the balance platform.
  name: balancePlatform
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-balance-account-notification-data-schema.json
slug: notification-webhooks-balance-account-notification-data
source_filename: notification-webhooks-balance-account-notification-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-balance-account-notification-data-schema.json\",\n  \"title\": \"BalanceAccountNotificationData\",\n  \"description\": \"BalanceAccountNotificationData schema from Adyen API\",\n  \"properties\": {\n    \"balanceAccount\": {\n      \"$ref\": \"#/components/schemas/BalanceAccount\"\n    },\n    \"balancePlatform\": {\n      \"description\": \"Unique identifier of the balance platform.\",\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-balance-account-notification-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BalanceAccountNotificationData
---
