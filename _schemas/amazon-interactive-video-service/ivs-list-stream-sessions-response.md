---
description: ListStreamSessionsResponse schema
layout: schema
name: ListStreamSessionsResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: streamSessions
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-list-stream-sessions-response-schema.json
slug: ivs-list-stream-sessions-response
source_filename: ivs-list-stream-sessions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-list-stream-sessions-response-schema.json\",\n  \"title\": \"ListStreamSessionsResponse\",\n  \"description\": \"ListStreamSessionsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"If there are more streams than <code>maxResults</code>, use <code>nextToken</code> in the request to get the next set.\"\n        }\n      ]\n    },\n    \"streamSessions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamSessionList\"\n        },\n        {\n          \"description\": \"List of stream sessions.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"streamSessions\"\n\
  \  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-list-stream-sessions-response-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: ListStreamSessionsResponse
---
