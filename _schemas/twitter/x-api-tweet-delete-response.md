---
description: TweetDeleteResponse schema from X API v2
layout: schema
name: TweetDeleteResponse
properties_list:
- description: ''
  name: data
  type: object
- description: ''
  name: errors
  type: array
provider_name: X (Twitter)
provider_slug: twitter
schema_file: json-schema/x-api-tweet-delete-response-schema.json
slug: x-api-tweet-delete-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-tweet-delete-response-schema.json\",\n  \"title\": \"TweetDeleteResponse\",\n  \"description\": \"TweetDeleteResponse schema from X API v2\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"deleted\"\n      ],\n      \"properties\": {\n        \"deleted\": {\n          \"type\": \"boolean\"\n        }\n      }\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Problem\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-tweet-delete-response-schema.json
tags:
- Social Media
- Microblogging
- Real-Time Data
- Streaming
- Advertising
- Content
title: TweetDeleteResponse
---
