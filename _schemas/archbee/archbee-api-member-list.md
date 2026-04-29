---
description: ''
layout: schema
name: MemberList
properties_list:
- description: ''
  name: members
  type: array
- description: Total number of members
  name: totalCount
  type: integer
provider_name: Archbee
provider_slug: archbee
schema_file: json-schema/archbee-api-member-list-schema.json
slug: archbee-api-member-list
source_filename: archbee-api-member-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"members\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {},\n          \"email\": {},\n          \"name\": {},\n          \"role\": {}\n        }\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of members\",\n      \"example\": 5\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/json-schema/archbee-api-member-list-schema.json\",\n  \"title\": \"MemberList\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/json-schema/archbee-api-member-list-schema.json
tags:
- API Documentation
- Documentation Platform
- Knowledge Base
- Technical Writing
- Developer Docs
title: MemberList
---
