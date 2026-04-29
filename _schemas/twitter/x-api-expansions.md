---
description: Expansions schema from X API v2
layout: schema
name: Expansions
properties_list:
- description: ''
  name: media
  type: array
- description: ''
  name: places
  type: array
- description: ''
  name: polls
  type: array
- description: ''
  name: topics
  type: array
- description: ''
  name: tweets
  type: array
- description: ''
  name: users
  type: array
provider_name: X (Twitter)
provider_slug: twitter
schema_file: json-schema/x-api-expansions-schema.json
slug: x-api-expansions
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-expansions-schema.json\",\n  \"title\": \"Expansions\",\n  \"description\": \"Expansions schema from X API v2\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"media\": {\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Media\"\n      }\n    },\n    \"places\": {\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Place\"\n      }\n    },\n    \"polls\": {\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Poll\"\n      }\n    },\n    \"topics\": {\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Topic\"\n      }\n    },\n    \"tweets\": {\n      \"\
  type\": \"array\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Tweet\"\n      }\n    },\n    \"users\": {\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/User\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-expansions-schema.json
tags:
- Social Media
- Microblogging
- Real-Time Data
- Streaming
- Advertising
- Content
title: Expansions
---
