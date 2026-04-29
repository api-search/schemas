---
description: Funds transfer response
layout: schema
name: FundsTransferResponse
properties_list:
- description: ''
  name: transferId
  type: string
- description: ''
  name: clientReference
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: amount
  type: number
- description: ''
  name: currency
  type: string
- description: ''
  name: debitAccountId
  type: string
- description: ''
  name: creditAccountId
  type: string
- description: ''
  name: valueDate
  type: string
- description: ''
  name: createdAt
  type: string
provider_name: BNY Mellon
provider_slug: bank-of-new-york-mellon
schema_file: json-schema/fundstransferresponse-schema.json
slug: fundstransferresponse
source_filename: fundstransferresponse-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bank-of-new-york-mellon/json-schema/fundstransferresponse-schema.json\",\n  \"title\": \"FundsTransferResponse\",\n  \"type\": \"object\",\n  \"description\": \"Funds transfer response\",\n  \"properties\": {\n    \"transferId\": {\n      \"type\": \"string\"\n    },\n    \"clientReference\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pending\",\n        \"processing\",\n        \"completed\",\n        \"rejected\"\n      ]\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"currency\": {\n      \"type\": \"string\"\n    },\n    \"debitAccountId\": {\n      \"type\": \"string\"\n    },\n    \"creditAccountId\": {\n      \"type\": \"string\"\n    },\n    \"valueDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"\
  createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bank-of-new-york-mellon/refs/heads/main/json-schema/fundstransferresponse-schema.json
tags:
- Asset Servicing
- Banking
- Institutional Banking
- Payments
- Treasury
- Wire Transfers
title: FundsTransferResponse
---
