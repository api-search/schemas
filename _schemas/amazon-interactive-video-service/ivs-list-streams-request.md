---
description: ListStreamsRequest schema
layout: schema
name: ListStreamsRequest
properties_list:
- description: ''
  name: filterBy
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-list-streams-request-schema.json
slug: ivs-list-streams-request
source_filename: ivs-list-streams-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-list-streams-request-schema.json\",\n  \"title\": \"ListStreamsRequest\",\n  \"description\": \"ListStreamsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filterBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamFilters\"\n        },\n        {\n          \"description\": \"Filters the stream list to match the specified criterion.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxStreamResults\"\n        },\n        {\n          \"description\": \"Maximum number of streams to return. Default: 100.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n\
  \        },\n        {\n          \"description\": \"The first stream to retrieve. This is used for pagination; see the <code>nextToken</code> response field.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-list-streams-request-schema.json
tags:
- Live Streaming
- Media
- Video
- Real-Time
title: ListStreamsRequest
---
