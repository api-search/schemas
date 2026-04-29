---
description: CreateTransactionModel schema from Avalara API
layout: schema
name: CreateTransactionModel
properties_list:
- description: The type of document to create
  name: type
  type: string
- description: Company code of the company creating this transaction
  name: companyCode
  type: string
- description: Date of the transaction
  name: date
  type: string
- description: Unique code identifying the customer
  name: customerCode
  type: string
- description: Whether to commit the transaction immediately
  name: commit
  type: boolean
- description: Three-character ISO 4217 currency code
  name: currencyCode
  type: string
- description: ''
  name: addresses
  type: object
- description: Line items for the transaction
  name: lines
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-create-transaction-model-schema.json
slug: avatax-rest-create-transaction-model
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-create-transaction-model-schema.json\",\n  \"title\": \"CreateTransactionModel\",\n  \"description\": \"CreateTransactionModel schema from Avalara API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"type\",\n    \"companyCode\",\n    \"date\",\n    \"customerCode\",\n    \"lines\"\n  ],\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SalesOrder\",\n        \"SalesInvoice\",\n        \"PurchaseOrder\",\n        \"PurchaseInvoice\",\n        \"ReturnOrder\",\n        \"ReturnInvoice\"\n      ],\n      \"description\": \"The type of document to create\"\n    },\n    \"companyCode\": {\n      \"type\": \"string\",\n      \"description\": \"Company code of the company creating this transaction\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n\
  \      \"format\": \"date\",\n      \"description\": \"Date of the transaction\"\n    },\n    \"customerCode\": {\n      \"type\": \"string\",\n      \"description\": \"Unique code identifying the customer\"\n    },\n    \"commit\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Whether to commit the transaction immediately\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"Three-character ISO 4217 currency code\"\n    },\n    \"addresses\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"shipFrom\": {\n          \"$ref\": \"#/components/schemas/AddressInfo\"\n        },\n        \"shipTo\": {\n          \"$ref\": \"#/components/schemas/AddressInfo\"\n        },\n        \"pointOfOrderOrigin\": {\n          \"$ref\": \"#/components/schemas/AddressInfo\"\n        },\n        \"pointOfOrderAcceptance\": {\n          \"$ref\": \"#/components/schemas/AddressInfo\"\n        }\n      }\n    },\n \
  \   \"lines\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LineItemModel\"\n      },\n      \"description\": \"Line items for the transaction\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-create-transaction-model-schema.json
tags:
- Taxes
title: CreateTransactionModel
---
