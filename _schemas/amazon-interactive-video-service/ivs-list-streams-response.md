---
description: ListStreamsResponse schema
layout: schema
name: ListStreamsResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: streams
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-list-streams-response-schema.json
slug: ivs-list-streams-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-list-streams-response-schema.json\",\n  \"title\": \"ListStreamsResponse\",\n  \"description\": \"ListStreamsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"If there are more streams than <code>maxResults</code>, use <code>nextToken</code> in the request to get the next set.\"\n        }\n      ]\n    },\n    \"streams\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamList\"\n        },\n        {\n          \"description\": \"List of streams.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"streams\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-list-streams-response-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: ListStreamsResponse
---
