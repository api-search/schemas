---
description: ListStreamKeysRequest schema
layout: schema
name: ListStreamKeysRequest
properties_list:
- description: ''
  name: channelArn
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-list-stream-keys-request-schema.json
slug: ivs-list-stream-keys-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-list-stream-keys-request-schema.json\",\n  \"title\": \"ListStreamKeysRequest\",\n  \"description\": \"ListStreamKeysRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"channelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChannelArn\"\n        },\n        {\n          \"description\": \"Channel ARN used to filter the list.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxStreamKeyResults\"\n        },\n        {\n          \"description\": \"Maximum number of streamKeys to return. Default: 1.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n\
  \        {\n          \"description\": \"The first stream key to retrieve. This is used for pagination; see the <code>nextToken</code> response field.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"channelArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-list-stream-keys-request-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: ListStreamKeysRequest
---
