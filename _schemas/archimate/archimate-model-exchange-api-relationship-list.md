---
description: ''
layout: schema
name: RelationshipList
properties_list:
- description: ''
  name: relationships
  type: array
- description: Total relationship count
  name: totalCount
  type: integer
provider_name: ArchiMate
provider_slug: archimate
schema_file: json-schema/archimate-model-exchange-api-relationship-list-schema.json
slug: archimate-model-exchange-api-relationship-list
source_filename: archimate-model-exchange-api-relationship-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"relationships\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {},\n          \"type\": {},\n          \"sourceId\": {},\n          \"targetId\": {},\n          \"label\": {}\n        }\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total relationship count\",\n      \"example\": 120\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archimate/refs/heads/main/json-schema/archimate-model-exchange-api-relationship-list-schema.json\",\n  \"title\": \"RelationshipList\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archimate/refs/heads/main/json-schema/archimate-model-exchange-api-relationship-list-schema.json
tags:
- Enterprise Architecture
- Architecture Framework
- Modeling Language
- Business Architecture
- Technology Architecture
- Standard
- Open Group
title: RelationshipList
---
