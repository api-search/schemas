---
description: Payment response
layout: schema
name: PaymentResponse
properties_list:
- description: ''
  name: paymentId
  type: string
- description: ''
  name: clientReference
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: paymentType
  type: string
- description: ''
  name: amount
  type: number
- description: ''
  name: currency
  type: string
- description: ''
  name: valueDate
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: statusMessage
  type: string
provider_name: BNY Mellon
provider_slug: bank-of-new-york-mellon
schema_file: json-schema/paymentresponse-schema.json
slug: paymentresponse
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bank-of-new-york-mellon/json-schema/paymentresponse-schema.json\",\n  \"title\": \"PaymentResponse\",\n  \"type\": \"object\",\n  \"description\": \"Payment response\",\n  \"properties\": {\n    \"paymentId\": {\n      \"type\": \"string\"\n    },\n    \"clientReference\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pending\",\n        \"processing\",\n        \"completed\",\n        \"rejected\",\n        \"returned\"\n      ]\n    },\n    \"paymentType\": {\n      \"type\": \"string\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"currency\": {\n      \"type\": \"string\"\n    },\n    \"valueDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"\
  date-time\"\n    },\n    \"statusMessage\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bank-of-new-york-mellon/refs/heads/main/json-schema/paymentresponse-schema.json
tags:
- Asset Servicing
- Banking
- Institutional Banking
- Payments
- Treasury
- Wire Transfers
title: PaymentResponse
---
