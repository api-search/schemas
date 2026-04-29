---
description: Error schema from X API v2
layout: schema
name: Error
properties_list:
- description: ''
  name: code
  type: integer
- description: ''
  name: message
  type: string
provider_name: X (Twitter)
provider_slug: twitter
schema_file: json-schema/x-api-error-schema.json
slug: x-api-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-error-schema.json\",\n  \"title\": \"Error\",\n  \"description\": \"Error schema from X API v2\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"code\",\n    \"message\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-error-schema.json
tags:
- Social Media
- Microblogging
- Real-Time Data
- Streaming
- Advertising
- Content
title: Error
---
