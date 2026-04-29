---
description: ''
layout: schema
name: ApInvoiceLine
properties_list:
- description: Invoice line number
  name: lineNumber
  type: integer
- description: Line type lookup code
  name: lineType
  type: string
- description: Line amount
  name: amount
  type: number
- description: Line description
  name: description
  type: string
- description: ''
  name: accountingDate
  type: string
- description: Distribution account code combination ID
  name: distCodeCombinationId
  type: integer
- description: ''
  name: itemDescription
  type: string
- description: ''
  name: quantity
  type: number
- description: ''
  name: unitPrice
  type: number
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/financial-services-ap-invoice-line-schema.json
slug: financial-services-ap-invoice-line
source_filename: financial-services-ap-invoice-line-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApInvoiceLine\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lineNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"Invoice line number\"\n    },\n    \"lineType\": {\n      \"type\": \"string\",\n      \"description\": \"Line type lookup code\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"Line amount\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Line description\"\n    },\n    \"accountingDate\": {\n      \"type\": \"string\"\n    },\n    \"distCodeCombinationId\": {\n      \"type\": \"integer\",\n      \"description\": \"Distribution account code combination ID\"\n    },\n    \"itemDescription\": {\n      \"type\": \"string\"\n    },\n    \"quantity\": {\n      \"type\": \"number\"\n    },\n    \"unitPrice\": {\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/financial-services-ap-invoice-line-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: ApInvoiceLine
---
