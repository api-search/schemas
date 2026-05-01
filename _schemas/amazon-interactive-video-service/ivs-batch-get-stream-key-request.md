---
description: BatchGetStreamKeyRequest schema
layout: schema
name: BatchGetStreamKeyRequest
properties_list:
- description: ''
  name: arns
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-batch-get-stream-key-request-schema.json
slug: ivs-batch-get-stream-key-request
source_filename: ivs-batch-get-stream-key-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-batch-get-stream-key-request-schema.json\",\n  \"title\": \"BatchGetStreamKeyRequest\",\n  \"description\": \"BatchGetStreamKeyRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamKeyArnList\"\n        },\n        {\n          \"description\": \"Array of ARNs, one per stream key.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arns\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-batch-get-stream-key-request-schema.json
tags:
- Live Streaming
- Media
- Video
- Real-Time
title: BatchGetStreamKeyRequest
---
