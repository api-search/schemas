---
description: ''
layout: schema
name: ArReceipt
properties_list:
- description: Cash receipt identifier
  name: cashReceiptId
  type: integer
- description: Receipt number
  name: receiptNumber
  type: string
- description: Receipt amount
  name: amount
  type: number
- description: Receipt currency code
  name: currencyCode
  type: string
- description: Receipt date
  name: receiptDate
  type: string
- description: Customer identifier
  name: customerId
  type: integer
- description: Customer name
  name: customerName
  type: string
- description: Receipt method identifier
  name: receiptMethodId
  type: integer
- description: Receipt status
  name: status
  type: string
- description: ''
  name: orgId
  type: integer
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/financial-services-ar-receipt-schema.json
slug: financial-services-ar-receipt
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ArReceipt\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cashReceiptId\": {\n      \"type\": \"integer\",\n      \"description\": \"Cash receipt identifier\"\n    },\n    \"receiptNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Receipt number\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"Receipt amount\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"Receipt currency code\"\n    },\n    \"receiptDate\": {\n      \"type\": \"string\",\n      \"description\": \"Receipt date\"\n    },\n    \"customerId\": {\n      \"type\": \"integer\",\n      \"description\": \"Customer identifier\"\n    },\n    \"customerName\": {\n      \"type\": \"string\",\n      \"description\": \"Customer name\"\n    },\n    \"receiptMethodId\": {\n      \"type\": \"integer\",\n      \"description\": \"Receipt method\
  \ identifier\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Receipt status\"\n    },\n    \"orgId\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/financial-services-ar-receipt-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: ArReceipt
---
