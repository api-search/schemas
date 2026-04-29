---
description: ListStreamKeysResponse schema
layout: schema
name: ListStreamKeysResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: streamKeys
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-list-stream-keys-response-schema.json
slug: ivs-list-stream-keys-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-list-stream-keys-response-schema.json\",\n  \"title\": \"ListStreamKeysResponse\",\n  \"description\": \"ListStreamKeysResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"If there are more stream keys than <code>maxResults</code>, use <code>nextToken</code> in the request to get the next set.\"\n        }\n      ]\n    },\n    \"streamKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamKeyList\"\n        },\n        {\n          \"description\": \"List of stream keys.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"streamKeys\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-list-stream-keys-response-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: ListStreamKeysResponse
---
