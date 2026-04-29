---
description: TSPairModel schema from Avalara API
layout: schema
name: TSPairModel
properties_list:
- description: Transaction type ID
  name: TransactionType
  type: integer
- description: ''
  name: TransactionTypeDescription
  type: string
- description: Service type ID
  name: ServiceType
  type: integer
- description: ''
  name: ServiceTypeDescription
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/communications-ts-pair-model-schema.json
slug: communications-ts-pair-model
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-ts-pair-model-schema.json\",\n  \"title\": \"TSPairModel\",\n  \"description\": \"TSPairModel schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TransactionType\": {\n      \"type\": \"integer\",\n      \"description\": \"Transaction type ID\"\n    },\n    \"TransactionTypeDescription\": {\n      \"type\": \"string\"\n    },\n    \"ServiceType\": {\n      \"type\": \"integer\",\n      \"description\": \"Service type ID\"\n    },\n    \"ServiceTypeDescription\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-ts-pair-model-schema.json
tags:
- Taxes
title: TSPairModel
---
