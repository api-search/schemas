---
description: InvoiceResponse schema from Avalara API
layout: schema
name: InvoiceResponse
properties_list:
- description: ''
  name: invoiceId
  type: string
- description: 44-digit NF-e access key
  name: accessKey
  type: string
- description: ''
  name: invoiceNumber
  type: integer
- description: ''
  name: series
  type: integer
- description: ''
  name: status
  type: string
- description: ''
  name: protocolNumber
  type: string
- description: ''
  name: issuanceDate
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-brazil-invoice-response-schema.json
slug: avatax-brazil-invoice-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-brazil-invoice-response-schema.json\",\n  \"title\": \"InvoiceResponse\",\n  \"description\": \"InvoiceResponse schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"invoiceId\": {\n      \"type\": \"string\"\n    },\n    \"accessKey\": {\n      \"type\": \"string\",\n      \"description\": \"44-digit NF-e access key\"\n    },\n    \"invoiceNumber\": {\n      \"type\": \"integer\"\n    },\n    \"series\": {\n      \"type\": \"integer\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Authorized\",\n        \"Cancelled\",\n        \"Denied\",\n        \"Pending\"\n      ]\n    },\n    \"protocolNumber\": {\n      \"type\": \"string\"\n    },\n    \"issuanceDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-brazil-invoice-response-schema.json
tags:
- Taxes
title: InvoiceResponse
---
