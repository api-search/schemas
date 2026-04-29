---
description: TransactionSummary schema from Avalara API
layout: schema
name: TransactionSummary
properties_list:
- description: ''
  name: country
  type: string
- description: ''
  name: region
  type: string
- description: ''
  name: jurisType
  type: string
- description: ''
  name: jurisCode
  type: string
- description: ''
  name: jurisName
  type: string
- description: ''
  name: taxType
  type: string
- description: ''
  name: rate
  type: number
- description: ''
  name: tax
  type: number
- description: ''
  name: taxable
  type: number
- description: ''
  name: exempt
  type: number
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-transaction-summary-schema.json
slug: avatax-rest-transaction-summary
source_filename: avatax-rest-transaction-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-transaction-summary-schema.json\",\n  \"title\": \"TransactionSummary\",\n  \"description\": \"TransactionSummary schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"country\": {\n      \"type\": \"string\"\n    },\n    \"region\": {\n      \"type\": \"string\"\n    },\n    \"jurisType\": {\n      \"type\": \"string\"\n    },\n    \"jurisCode\": {\n      \"type\": \"string\"\n    },\n    \"jurisName\": {\n      \"type\": \"string\"\n    },\n    \"taxType\": {\n      \"type\": \"string\"\n    },\n    \"rate\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"tax\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"taxable\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"exempt\": {\n      \"\
  type\": \"number\",\n      \"format\": \"double\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-transaction-summary-schema.json
tags:
- Taxes
title: TransactionSummary
---
