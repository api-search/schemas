---
description: TransferNotificationValidationFact schema from Adyen API
layout: schema
name: TransferNotificationValidationFact
properties_list:
- description: The evaluation result of the validation fact.
  name: result
  type: string
- description: The type of the validation fact.
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfers-transfer-notification-validation-fact-schema.json
slug: transfers-transfer-notification-validation-fact
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-transfer-notification-validation-fact-schema.json\",\n  \"title\": \"TransferNotificationValidationFact\",\n  \"description\": \"TransferNotificationValidationFact schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"result\": {\n      \"description\": \"The evaluation result of the validation fact.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The type of the validation fact.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-transfer-notification-validation-fact-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransferNotificationValidationFact
---
