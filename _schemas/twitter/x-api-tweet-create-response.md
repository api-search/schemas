---
description: TweetCreateResponse schema from X API v2
layout: schema
name: TweetCreateResponse
properties_list:
- description: ''
  name: data
  type: object
- description: ''
  name: errors
  type: array
provider_name: X (Twitter)
provider_slug: twitter
schema_file: json-schema/x-api-tweet-create-response-schema.json
slug: x-api-tweet-create-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-tweet-create-response-schema.json\",\n  \"title\": \"TweetCreateResponse\",\n  \"description\": \"TweetCreateResponse schema from X API v2\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"id\",\n        \"text\"\n      ],\n      \"properties\": {\n        \"id\": {\n          \"$ref\": \"#/components/schemas/TweetId\"\n        },\n        \"text\": {\n          \"$ref\": \"#/components/schemas/TweetText\"\n        }\n      }\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Problem\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-tweet-create-response-schema.json
tags:
- Social Media
- Microblogging
- Real-Time Data
- Streaming
- Advertising
- Content
title: TweetCreateResponse
---
