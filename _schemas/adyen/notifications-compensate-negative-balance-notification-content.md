---
description: CompensateNegativeBalanceNotificationContent schema from Adyen API
layout: schema
name: CompensateNegativeBalanceNotificationContent
properties_list:
- description: A list of the negative balances compensated.
  name: records
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-compensate-negative-balance-notification-content-schema.json
slug: notifications-compensate-negative-balance-notification-content
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-compensate-negative-balance-notification-content-schema.json\",\n  \"title\": \"CompensateNegativeBalanceNotificationContent\",\n  \"description\": \"CompensateNegativeBalanceNotificationContent schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"records\": {\n      \"description\": \"A list of the negative balances compensated.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CompensateNegativeBalanceNotificationRecord\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-compensate-negative-balance-notification-content-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CompensateNegativeBalanceNotificationContent
---
