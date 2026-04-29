---
description: BalanceAccountNotificationData schema from Adyen API
layout: schema
name: BalanceAccountNotificationData
properties_list:
- description: ''
  name: balanceAccount
  type: object
- description: The unique identifier of the balance platform.
  name: balancePlatform
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-webhooks-balance-account-notification-data-schema.json
slug: configuration-webhooks-balance-account-notification-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-balance-account-notification-data-schema.json\",\n  \"title\": \"BalanceAccountNotificationData\",\n  \"description\": \"BalanceAccountNotificationData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"balanceAccount\": {\n      \"$ref\": \"#/components/schemas/BalanceAccount\"\n    },\n    \"balancePlatform\": {\n      \"description\": \"The unique identifier of the balance platform.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-balance-account-notification-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BalanceAccountNotificationData
---
