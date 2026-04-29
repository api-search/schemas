---
description: ''
layout: schema
name: SpaceList
properties_list:
- description: ''
  name: spaces
  type: array
- description: Total number of spaces
  name: totalCount
  type: integer
provider_name: Archbee
provider_slug: archbee
schema_file: json-schema/archbee-api-space-list-schema.json
slug: archbee-api-space-list
source_filename: archbee-api-space-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"spaces\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {},\n          \"name\": {},\n          \"slug\": {},\n          \"visibility\": {},\n          \"description\": {},\n          \"pageCount\": {},\n          \"createdAt\": {}\n        }\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of spaces\",\n      \"example\": 3\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/json-schema/archbee-api-space-list-schema.json\",\n  \"title\": \"SpaceList\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/json-schema/archbee-api-space-list-schema.json
tags:
- API Documentation
- Documentation Platform
- Knowledge Base
- Technical Writing
- Developer Docs
title: SpaceList
---
