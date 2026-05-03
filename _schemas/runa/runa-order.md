---
description: A digital reward or gift card order on the Runa platform
layout: schema
name: Runa Order
properties_list:
- description: Unique order identifier
  name: id
  type: string
- description: Order fulfillment status
  name: status
  type: string
- description: Order creation timestamp
  name: created_at
  type: string
- description: Order completion timestamp
  name: completed_at
  type: string
- description: Payment source used
  name: payment_method
  type: object
- description: Order line items with fulfillment details
  name: items
  type: array
provider_name: Runa
provider_slug: runa
schema_file: json-schema/runa-order-schema.json
slug: runa-order
source_filename: runa-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.runa.io/schemas/order\",\n  \"title\": \"Runa Order\",\n  \"description\": \"A digital reward or gift card order on the Runa platform\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique order identifier\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Order fulfillment status\",\n      \"enum\": [\"PENDING\", \"PROCESSING\", \"COMPLETED\", \"FAILED\", \"CANCELLED\"]\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Order creation timestamp\"\n    },\n    \"completed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Order completion timestamp\"\n    },\n    \"payment_method\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Payment source used\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"ACCOUNT_BALANCE\"]\n        },\n        \"currency\": {\n          \"type\": \"string\",\n          \"description\": \"ISO 4217 currency code\"\n        }\n      }\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"Order line items with fulfillment details\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"string\", \"description\": \"Item identifier\" },\n          \"face_value\": { \"type\": \"number\", \"description\": \"Item face value\" },\n          \"currency\": { \"type\": \"string\", \"description\": \"Item currency\" },\n          \"status\": { \"type\": \"string\", \"description\": \"Item status\" },\n          \"payout\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"url\": {\n                \"type\": \"string\",\n \
  \               \"format\": \"uri\",\n                \"description\": \"Payout redemption link\"\n              },\n              \"expires_at\": {\n                \"type\": \"string\",\n                \"format\": \"date-time\",\n                \"description\": \"Link expiration\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/runa/refs/heads/main/json-schema/runa-order-schema.json
tags:
- Gift Cards
- Rewards
- Payments
- Incentives
- Payouts
title: Runa Order
---
