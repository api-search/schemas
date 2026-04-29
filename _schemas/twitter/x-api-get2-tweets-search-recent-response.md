---
description: Get2TweetsSearchRecentResponse schema from X API v2
layout: schema
name: Get2TweetsSearchRecentResponse
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: errors
  type: array
- description: ''
  name: includes
  type: object
- description: ''
  name: meta
  type: object
provider_name: X (Twitter)
provider_slug: twitter
schema_file: json-schema/x-api-get2-tweets-search-recent-response-schema.json
slug: x-api-get2-tweets-search-recent-response
source_filename: x-api-get2-tweets-search-recent-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-get2-tweets-search-recent-response-schema.json\",\n  \"title\": \"Get2TweetsSearchRecentResponse\",\n  \"description\": \"Get2TweetsSearchRecentResponse schema from X API v2\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Tweet\"\n      }\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Problem\"\n      }\n    },\n    \"includes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"media\": {\n          \"type\": \"array\",\n          \"minItems\": 1,\n          \"items\": {\n            \"$ref\": \"#/components/schemas/Media\"\n          }\n        },\n        \"places\"\
  : {\n          \"type\": \"array\",\n          \"minItems\": 1,\n          \"items\": {\n            \"$ref\": \"#/components/schemas/Place\"\n          }\n        },\n        \"polls\": {\n          \"type\": \"array\",\n          \"minItems\": 1,\n          \"items\": {\n            \"$ref\": \"#/components/schemas/Poll\"\n          }\n        },\n        \"topics\": {\n          \"type\": \"array\",\n          \"minItems\": 1,\n          \"items\": {\n            \"$ref\": \"#/components/schemas/Topic\"\n          }\n        },\n        \"tweets\": {\n          \"type\": \"array\",\n          \"minItems\": 1,\n          \"items\": {\n            \"$ref\": \"#/components/schemas/Tweet\"\n          }\n        },\n        \"users\": {\n          \"type\": \"array\",\n          \"minItems\": 1,\n          \"items\": {\n            \"$ref\": \"#/components/schemas/User\"\n          }\n        }\n      }\n    },\n    \"meta\": {\n      \"type\": \"object\",\n      \"properties\": {\n    \
  \    \"newest_id\": {\n          \"$ref\": \"#/components/schemas/NewestId\"\n        },\n        \"next_token\": {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        \"oldest_id\": {\n          \"$ref\": \"#/components/schemas/OldestId\"\n        },\n        \"result_count\": {\n          \"$ref\": \"#/components/schemas/ResultCount\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-get2-tweets-search-recent-response-schema.json
tags:
- Social Media
- Microblogging
- Real-Time Data
- Streaming
- Advertising
- Content
title: Get2TweetsSearchRecentResponse
---
