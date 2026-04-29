---
description: CompensateNegativeBalanceNotificationRecord schema from Adyen API
layout: schema
name: CompensateNegativeBalanceNotificationRecord
properties_list:
- description: The code of the account whose negative balance has been compensated.
  name: accountCode
  type: string
- description: The amount compensated.
  name: amount
  type: object
- description: The date on which the compensation took place.
  name: transferDate
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-compensate-negative-balance-notification-record-schema.json
slug: notifications-compensate-negative-balance-notification-record
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-compensate-negative-balance-notification-record-schema.json\",\n  \"title\": \"CompensateNegativeBalanceNotificationRecord\",\n  \"description\": \"CompensateNegativeBalanceNotificationRecord schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountCode\": {\n      \"description\": \"The code of the account whose negative balance has been compensated.\",\n      \"type\": \"string\"\n    },\n    \"amount\": {\n      \"description\": \"The amount compensated.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"transferDate\": {\n      \"description\": \"The date on which the compensation took place.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-compensate-negative-balance-notification-record-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CompensateNegativeBalanceNotificationRecord
---
