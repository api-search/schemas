---
description: List of payments
layout: schema
name: PaymentListResponse
properties_list:
- description: ''
  name: payments
  type: array
- description: ''
  name: totalCount
  type: integer
provider_name: BNY Mellon
provider_slug: bank-of-new-york-mellon
schema_file: json-schema/paymentlistresponse-schema.json
slug: paymentlistresponse
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bank-of-new-york-mellon/json-schema/paymentlistresponse-schema.json\",\n  \"title\": \"PaymentListResponse\",\n  \"type\": \"object\",\n  \"description\": \"List of payments\",\n  \"properties\": {\n    \"payments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PaymentResponse\"\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bank-of-new-york-mellon/refs/heads/main/json-schema/paymentlistresponse-schema.json
tags:
- Asset Servicing
- Banking
- Institutional Banking
- Payments
- Treasury
- Wire Transfers
title: PaymentListResponse
---
