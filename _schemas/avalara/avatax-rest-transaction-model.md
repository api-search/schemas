---
description: TransactionModel schema from Avalara API
layout: schema
name: TransactionModel
properties_list:
- description: Unique ID of the transaction
  name: id
  type: integer
- description: Transaction code
  name: code
  type: string
- description: Company ID that owns this transaction
  name: companyId
  type: integer
- description: Date of the transaction
  name: date
  type: string
- description: Current status of the transaction
  name: status
  type: string
- description: Document type
  name: type
  type: string
- description: Total amount of the transaction before tax
  name: totalAmount
  type: number
- description: Total tax calculated for the transaction
  name: totalTax
  type: number
- description: Total taxable amount
  name: totalTaxable
  type: number
- description: Total exempt amount
  name: totalExempt
  type: number
- description: ''
  name: lines
  type: array
- description: ''
  name: addresses
  type: array
- description: ''
  name: summary
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-transaction-model-schema.json
slug: avatax-rest-transaction-model
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-transaction-model-schema.json\",\n  \"title\": \"TransactionModel\",\n  \"description\": \"TransactionModel schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Unique ID of the transaction\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction code\"\n    },\n    \"companyId\": {\n      \"type\": \"integer\",\n      \"description\": \"Company ID that owns this transaction\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of the transaction\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Temporary\",\n        \"Saved\",\n        \"Posted\"\
  ,\n        \"Committed\",\n        \"Cancelled\",\n        \"Adjusted\"\n      ],\n      \"description\": \"Current status of the transaction\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Document type\"\n    },\n    \"totalAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Total amount of the transaction before tax\"\n    },\n    \"totalTax\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Total tax calculated for the transaction\"\n    },\n    \"totalTaxable\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Total taxable amount\"\n    },\n    \"totalExempt\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Total exempt amount\"\n    },\n    \"lines\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TransactionLineModel\"\n      }\n    },\n\
  \    \"addresses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TransactionAddressModel\"\n      }\n    },\n    \"summary\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TransactionSummary\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-transaction-model-schema.json
tags:
- Taxes
title: TransactionModel
---
