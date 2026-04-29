---
description: TaxDeterminationRequest schema from Avalara API
layout: schema
name: TaxDeterminationRequest
properties_list:
- description: Date for tax determination
  name: effectiveDate
  type: string
- description: ''
  name: invoiceNumber
  type: string
- description: ''
  name: invoiceDate
  type: string
- description: Title transfer point
  name: titleTransferCode
  type: string
- description: Type of excise transaction
  name: transactionType
  type: string
- description: ''
  name: seller
  type: object
- description: ''
  name: buyer
  type: object
- description: ''
  name: transactionLines
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/excise-tax-determination-request-schema.json
slug: excise-tax-determination-request
source_filename: excise-tax-determination-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/excise-tax-determination-request-schema.json\",\n  \"title\": \"TaxDeterminationRequest\",\n  \"description\": \"TaxDeterminationRequest schema from Avalara API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"effectiveDate\",\n    \"transactionLines\"\n  ],\n  \"properties\": {\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date for tax determination\"\n    },\n    \"invoiceNumber\": {\n      \"type\": \"string\"\n    },\n    \"invoiceDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"titleTransferCode\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Origin\",\n        \"Destination\"\n      ],\n      \"description\": \"Title transfer point\"\n    },\n    \"transactionType\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Type of excise transaction\"\n    },\n    \"seller\": {\n      \"$ref\": \"#/components/schemas/TransactionParty\"\n    },\n    \"buyer\": {\n      \"$ref\": \"#/components/schemas/TransactionParty\"\n    },\n    \"transactionLines\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TransactionLine\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/excise-tax-determination-request-schema.json
tags:
- Taxes
title: TaxDeterminationRequest
---
