---
description: RefundTransactionModel schema from Avalara API
layout: schema
name: RefundTransactionModel
properties_list:
- description: ''
  name: refundTransactionCode
  type: string
- description: ''
  name: refundDate
  type: string
- description: ''
  name: refundType
  type: string
- description: ''
  name: refundPercentage
  type: number
- description: ''
  name: refundLines
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-refund-transaction-model-schema.json
slug: avatax-rest-refund-transaction-model
source_filename: avatax-rest-refund-transaction-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-refund-transaction-model-schema.json\",\n  \"title\": \"RefundTransactionModel\",\n  \"description\": \"RefundTransactionModel schema from Avalara API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"refundTransactionCode\",\n    \"refundDate\",\n    \"refundType\"\n  ],\n  \"properties\": {\n    \"refundTransactionCode\": {\n      \"type\": \"string\"\n    },\n    \"refundDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"refundType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Full\",\n        \"Partial\",\n        \"Percentage\",\n        \"TaxOnly\"\n      ]\n    },\n    \"refundPercentage\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"refundLines\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"\
  type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-refund-transaction-model-schema.json
tags:
- Taxes
title: RefundTransactionModel
---
