---
description: ListStreamSessionsRequest schema
layout: schema
name: ListStreamSessionsRequest
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
schema_file: json-schema/ivs-list-stream-sessions-request-schema.json
slug: ivs-list-stream-sessions-request
source_filename: ivs-list-stream-sessions-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-list-stream-sessions-request-schema.json\",\n  \"title\": \"ListStreamSessionsRequest\",\n  \"description\": \"ListStreamSessionsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"channelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChannelArn\"\n        },\n        {\n          \"description\": \"Channel ARN used to filter the list.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxStreamResults\"\n        },\n        {\n          \"description\": \"Maximum number of streams to return. Default: 100.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n\
  \        },\n        {\n          \"description\": \"The first stream to retrieve. This is used for pagination; see the <code>nextToken</code> response field.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"channelArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-list-stream-sessions-request-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: ListStreamSessionsRequest
---
