---
description: Amount schema from Adyen API
layout: schema
name: Amount
properties_list:
- description: The three-character [ISO currency code](https://docs.adyen.com/development-resources/currency-codes).
  name: currency
  type: string
- description: The amount of the transaction, in [minor units](https://docs.adyen.com/development-resources/currency-codes).
  name: value
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-amount-schema.json
slug: notification-webhooks-amount
source_filename: notification-webhooks-amount-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-amount-schema.json\",\n  \"title\": \"Amount\",\n  \"description\": \"Amount schema from Adyen API\",\n  \"properties\": {\n    \"currency\": {\n      \"description\": \"The three-character [ISO currency code](https://docs.adyen.com/development-resources/currency-codes).\",\n      \"maxLength\": 3,\n      \"minLength\": 3,\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"The amount of the transaction, in [minor units](https://docs.adyen.com/development-resources/currency-codes).\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"value\",\n    \"currency\"\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-amount-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Amount
---
