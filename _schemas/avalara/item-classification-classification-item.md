---
description: ClassificationItem schema from Avalara API
layout: schema
name: ClassificationItem
properties_list:
- description: Unique item identifier
  name: itemCode
  type: string
- description: Product description for classification
  name: description
  type: string
- description: Short product summary
  name: summary
  type: string
- description: Additional product attributes for classification
  name: attributes
  type: object
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/item-classification-classification-item-schema.json
slug: item-classification-classification-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/item-classification-classification-item-schema.json\",\n  \"title\": \"ClassificationItem\",\n  \"description\": \"ClassificationItem schema from Avalara API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"description\"\n  ],\n  \"properties\": {\n    \"itemCode\": {\n      \"type\": \"string\",\n      \"description\": \"Unique item identifier\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Product description for classification\"\n    },\n    \"summary\": {\n      \"type\": \"string\",\n      \"description\": \"Short product summary\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Additional product attributes for classification\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/item-classification-classification-item-schema.json
tags:
- Taxes
title: ClassificationItem
---
