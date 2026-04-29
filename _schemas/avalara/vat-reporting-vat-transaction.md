---
description: VATTransaction schema from Avalara API
layout: schema
name: VATTransaction
properties_list:
- description: ''
  name: transactionId
  type: string
- description: ''
  name: transactionDate
  type: string
- description: ''
  name: transactionType
  type: string
- description: ''
  name: invoiceNumber
  type: string
- description: ''
  name: supplierVATNumber
  type: string
- description: ''
  name: customerVATNumber
  type: string
- description: ''
  name: countryCode
  type: string
- description: ''
  name: netAmount
  type: number
- description: ''
  name: vatRate
  type: number
- description: ''
  name: vatAmount
  type: number
- description: ''
  name: currency
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/vat-reporting-vat-transaction-schema.json
slug: vat-reporting-vat-transaction
source_filename: vat-reporting-vat-transaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/vat-reporting-vat-transaction-schema.json\",\n  \"title\": \"VATTransaction\",\n  \"description\": \"VATTransaction schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"transactionId\": {\n      \"type\": \"string\"\n    },\n    \"transactionDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"transactionType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Sale\",\n        \"Purchase\",\n        \"IntraCommunitySupply\",\n        \"IntraCommunityAcquisition\",\n        \"Export\",\n        \"Import\"\n      ]\n    },\n    \"invoiceNumber\": {\n      \"type\": \"string\"\n    },\n    \"supplierVATNumber\": {\n      \"type\": \"string\"\n    },\n    \"customerVATNumber\": {\n      \"type\": \"string\"\n    },\n    \"countryCode\": {\n      \"\
  type\": \"string\"\n    },\n    \"netAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"vatRate\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"vatAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"currency\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/vat-reporting-vat-transaction-schema.json
tags:
- Taxes
title: VATTransaction
---
