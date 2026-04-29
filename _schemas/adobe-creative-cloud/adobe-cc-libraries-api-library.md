---
description: Library from Adobe API
layout: schema
name: Library
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: created_date
  type: string
- description: ''
  name: modified_date
  type: string
- description: ''
  name: owner
  type: object
- description: ''
  name: element_count
  type: integer
provider_name: Adobe Creative Cloud
provider_slug: adobe-creative-cloud
schema_file: json-schema/adobe-cc-libraries-api-library-schema.json
slug: adobe-cc-libraries-api-library
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-cc-libraries-api-library-schema.json\",\n  \"title\": \"Library\",\n  \"description\": \"Library from Adobe API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123def456\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Asset\"\n    },\n    \"created_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"modified_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"owner\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"user_id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\"\
  : \"string\"\n        }\n      }\n    },\n    \"element_count\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-cc-libraries-api-library-schema.json
tags:
- AI/ML
- Cloud
- Creative
- Design
- Documents
- Photography
- SaaS
- Video
title: Library
---
