---
description: DetailBalance schema from Adyen API
layout: schema
name: DetailBalance
properties_list:
- description: The list of balances held by the account.
  name: balance
  type: array
- description: The list of on hold balances held by the account.
  name: onHoldBalance
  type: array
- description: The list of pending balances held by the account.
  name: pendingBalance
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/funds-detail-balance-schema.json
slug: funds-detail-balance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-detail-balance-schema.json\",\n  \"title\": \"DetailBalance\",\n  \"description\": \"DetailBalance schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"balance\": {\n      \"description\": \"The list of balances held by the account.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Amount\"\n      },\n      \"type\": \"array\"\n    },\n    \"onHoldBalance\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"The list of on hold balances held by the account.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Amount\"\n      },\n      \"type\": \"array\"\n    },\n    \"pendingBalance\": {\n      \"description\": \"The list of pending balances held by the account.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Amount\"\n    \
  \  },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-detail-balance-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DetailBalance
---
