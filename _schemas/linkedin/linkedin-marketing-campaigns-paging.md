---
description: Paging from LinkedIn API
layout: schema
name: Paging
properties_list:
- description: ''
  name: start
  type: integer
- description: ''
  name: count
  type: integer
- description: ''
  name: total
  type: integer
- description: ''
  name: links
  type: array
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-campaigns-paging-schema.json
slug: linkedin-marketing-campaigns-paging
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-campaigns-paging-schema.json\",\n  \"title\": \"Paging\",\n  \"description\": \"Paging from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"start\": {\n      \"type\": \"integer\",\n      \"example\": 0\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"links\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-campaigns-paging-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: Paging
---
