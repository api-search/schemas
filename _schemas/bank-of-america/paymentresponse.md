---
description: Payment transaction response
layout: schema
name: PaymentResponse
properties_list:
- description: Unique payment identifier
  name: paymentId
  type: string
- description: Client-provided reference
  name: clientReferenceId
  type: string
- description: Payment status
  name: status
  type: string
- description: Payment type
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
  name: updatedAt
  type: string
- description: Additional status information
  name: statusMessage
  type: string
provider_name: Bank of America
provider_slug: bank-of-america
schema_file: json-schema/paymentresponse-schema.json
slug: paymentresponse
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bank-of-america/json-schema/paymentresponse-schema.json\",\n  \"title\": \"PaymentResponse\",\n  \"type\": \"object\",\n  \"description\": \"Payment transaction response\",\n  \"properties\": {\n    \"paymentId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique payment identifier\"\n    },\n    \"clientReferenceId\": {\n      \"type\": \"string\",\n      \"description\": \"Client-provided reference\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Payment status\",\n      \"enum\": [\n        \"pending\",\n        \"processing\",\n        \"completed\",\n        \"rejected\",\n        \"cancelled\"\n      ]\n    },\n    \"paymentType\": {\n      \"type\": \"string\",\n      \"description\": \"Payment type\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"currency\"\
  : {\n      \"type\": \"string\"\n    },\n    \"valueDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"statusMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Additional status information\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bank-of-america/refs/heads/main/json-schema/paymentresponse-schema.json
tags:
- Banking
- Corporate Banking
- Finance
- Payments
- Treasury
- CashPro
title: PaymentResponse
---
