---
description: ''
layout: schema
name: ModelList
properties_list:
- description: ''
  name: models
  type: array
- description: Total number of models
  name: totalCount
  type: integer
provider_name: ArchiMate
provider_slug: archimate
schema_file: json-schema/archimate-model-exchange-api-model-list-schema.json
slug: archimate-model-exchange-api-model-list
source_filename: archimate-model-exchange-api-model-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"models\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {},\n          \"name\": {},\n          \"version\": {},\n          \"language\": {},\n          \"createdAt\": {},\n          \"modifiedAt\": {}\n        }\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of models\",\n      \"example\": 5\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archimate/refs/heads/main/json-schema/archimate-model-exchange-api-model-list-schema.json\",\n  \"title\": \"ModelList\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archimate/refs/heads/main/json-schema/archimate-model-exchange-api-model-list-schema.json
tags:
- Enterprise Architecture
- Architecture Framework
- Modeling Language
- Business Architecture
- Technology Architecture
- Standard
- Open Group
title: ModelList
---
