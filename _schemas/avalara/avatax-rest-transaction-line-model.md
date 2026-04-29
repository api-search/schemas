---
description: TransactionLineModel schema from Avalara API
layout: schema
name: TransactionLineModel
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: lineNumber
  type: string
- description: ''
  name: lineAmount
  type: number
- description: ''
  name: tax
  type: number
- description: ''
  name: taxableAmount
  type: number
- description: ''
  name: exemptAmount
  type: number
- description: ''
  name: taxCode
  type: string
- description: ''
  name: itemCode
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-transaction-line-model-schema.json
slug: avatax-rest-transaction-line-model
source_filename: avatax-rest-transaction-line-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-transaction-line-model-schema.json\",\n  \"title\": \"TransactionLineModel\",\n  \"description\": \"TransactionLineModel schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"lineNumber\": {\n      \"type\": \"string\"\n    },\n    \"lineAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"tax\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"taxableAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"exemptAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"taxCode\": {\n      \"type\": \"string\"\n    },\n    \"itemCode\": {\n      \"type\": \"string\"\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-transaction-line-model-schema.json
tags:
- Taxes
title: TransactionLineModel
---
