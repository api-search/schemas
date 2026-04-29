---
description: ''
layout: schema
name: ArInvoiceLine
properties_list:
- description: ''
  name: customerTrxLineId
  type: integer
- description: ''
  name: lineNumber
  type: integer
- description: ''
  name: lineType
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: quantity
  type: number
- description: ''
  name: unitSellingPrice
  type: number
- description: ''
  name: amount
  type: number
- description: ''
  name: inventoryItemId
  type: integer
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/financial-services-ar-invoice-line-schema.json
slug: financial-services-ar-invoice-line
source_filename: financial-services-ar-invoice-line-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ArInvoiceLine\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"customerTrxLineId\": {\n      \"type\": \"integer\"\n    },\n    \"lineNumber\": {\n      \"type\": \"integer\"\n    },\n    \"lineType\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"quantity\": {\n      \"type\": \"number\"\n    },\n    \"unitSellingPrice\": {\n      \"type\": \"number\"\n    },\n    \"amount\": {\n      \"type\": \"number\"\n    },\n    \"inventoryItemId\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/financial-services-ar-invoice-line-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: ArInvoiceLine
---
