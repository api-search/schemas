---
description: InvoiceLine schema from Avalara API
layout: schema
name: InvoiceLine
properties_list:
- description: ''
  name: lineNumber
  type: integer
- description: ''
  name: itemCode
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: quantity
  type: number
- description: ''
  name: unitPrice
  type: number
- description: ''
  name: ncmCode
  type: string
- description: ''
  name: cfopCode
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-brazil-invoice-line-schema.json
slug: avatax-brazil-invoice-line
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-brazil-invoice-line-schema.json\",\n  \"title\": \"InvoiceLine\",\n  \"description\": \"InvoiceLine schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lineNumber\": {\n      \"type\": \"integer\"\n    },\n    \"itemCode\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"quantity\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"unitPrice\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"ncmCode\": {\n      \"type\": \"string\"\n    },\n    \"cfopCode\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-brazil-invoice-line-schema.json
tags:
- Taxes
title: InvoiceLine
---
