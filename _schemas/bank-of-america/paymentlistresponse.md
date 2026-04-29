---
description: Paginated list of payments
layout: schema
name: PaymentListResponse
properties_list:
- description: ''
  name: payments
  type: array
- description: ''
  name: totalCount
  type: integer
- description: ''
  name: pageSize
  type: integer
- description: ''
  name: offset
  type: integer
provider_name: Bank of America
provider_slug: bank-of-america
schema_file: json-schema/paymentlistresponse-schema.json
slug: paymentlistresponse
source_filename: paymentlistresponse-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bank-of-america/json-schema/paymentlistresponse-schema.json\",\n  \"title\": \"PaymentListResponse\",\n  \"type\": \"object\",\n  \"description\": \"Paginated list of payments\",\n  \"properties\": {\n    \"payments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PaymentResponse\"\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\"\n    },\n    \"pageSize\": {\n      \"type\": \"integer\"\n    },\n    \"offset\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bank-of-america/refs/heads/main/json-schema/paymentlistresponse-schema.json
tags:
- Banking
- Corporate Banking
- Finance
- Payments
- Treasury
- CashPro
title: PaymentListResponse
---
