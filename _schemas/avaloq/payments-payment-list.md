---
description: Paginated list of payments
layout: schema
name: PaymentList
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: total
  type: integer
- description: ''
  name: offset
  type: integer
provider_name: Avaloq
provider_slug: avaloq
schema_file: json-schema/payments-payment-list-schema.json
slug: payments-payment-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/json-schema/payments-payment-list-schema.json\",\n  \"title\": \"PaymentList\",\n  \"description\": \"Paginated list of payments\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Payment\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"offset\": {\n      \"type\": \"integer\",\n      \"example\": 0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/json-schema/payments-payment-list-schema.json
tags:
- Banking
- Digital Banking
- Financial Services
- Fintech
- Payments
- Wealth Management
title: PaymentList
---
