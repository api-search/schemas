---
description: BatchGetStreamKeyResponse schema
layout: schema
name: BatchGetStreamKeyResponse
properties_list:
- description: ''
  name: errors
  type: object
- description: ''
  name: streamKeys
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-batch-get-stream-key-response-schema.json
slug: ivs-batch-get-stream-key-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-batch-get-stream-key-response-schema.json\",\n  \"title\": \"BatchGetStreamKeyResponse\",\n  \"description\": \"BatchGetStreamKeyResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchErrors\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    },\n    \"streamKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamKeys\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-batch-get-stream-key-response-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: BatchGetStreamKeyResponse
---
