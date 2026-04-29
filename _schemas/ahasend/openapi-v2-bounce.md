---
description: Bounce schema from AhaSend API
layout: schema
name: Bounce
properties_list:
- description: Bounce classification
  name: classification
  type: string
- description: Number of bounces
  name: count
  type: integer
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-bounce-schema.json
slug: openapi-v2-bounce
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-bounce-schema.json\",\n  \"title\": \"Bounce\",\n  \"description\": \"Bounce schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"classification\": {\n      \"type\": \"string\",\n      \"description\": \"Bounce classification\",\n      \"example\": \"example_value\"\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of bounces\",\n      \"example\": 1\n    }\n  },\n  \"required\": [\n    \"classification\",\n    \"count\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-bounce-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: Bounce
---
