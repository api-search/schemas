---
description: ''
layout: schema
name: PageList
properties_list:
- description: ''
  name: pages
  type: array
- description: Total number of pages
  name: totalCount
  type: integer
provider_name: Archbee
provider_slug: archbee
schema_file: json-schema/archbee-api-page-list-schema.json
slug: archbee-api-page-list
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"pages\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {},\n          \"title\": {},\n          \"slug\": {},\n          \"status\": {},\n          \"content\": {},\n          \"spaceId\": {},\n          \"parentId\": {},\n          \"updatedAt\": {}\n        }\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of pages\",\n      \"example\": 10\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/json-schema/archbee-api-page-list-schema.json\",\n  \"title\": \"PageList\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/json-schema/archbee-api-page-list-schema.json
tags:
- API Documentation
- Documentation Platform
- Knowledge Base
- Technical Writing
- Developer Docs
title: PageList
---
