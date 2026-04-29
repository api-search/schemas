---
description: ItemModel schema from Avalara API
layout: schema
name: ItemModel
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: companyId
  type: integer
- description: Unique code for this item
  name: itemCode
  type: string
- description: Avalara tax code for this item
  name: taxCode
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: category
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-item-model-schema.json
slug: avatax-rest-item-model
source_filename: avatax-rest-item-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-item-model-schema.json\",\n  \"title\": \"ItemModel\",\n  \"description\": \"ItemModel schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"companyId\": {\n      \"type\": \"integer\"\n    },\n    \"itemCode\": {\n      \"type\": \"string\",\n      \"description\": \"Unique code for this item\"\n    },\n    \"taxCode\": {\n      \"type\": \"string\",\n      \"description\": \"Avalara tax code for this item\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"category\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-item-model-schema.json
tags:
- Taxes
title: ItemModel
---
