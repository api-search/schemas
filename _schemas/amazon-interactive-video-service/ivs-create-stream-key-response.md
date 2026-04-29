---
description: CreateStreamKeyResponse schema
layout: schema
name: CreateStreamKeyResponse
properties_list:
- description: ''
  name: streamKey
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-create-stream-key-response-schema.json
slug: ivs-create-stream-key-response
source_filename: ivs-create-stream-key-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-create-stream-key-response-schema.json\",\n  \"title\": \"CreateStreamKeyResponse\",\n  \"description\": \"CreateStreamKeyResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"streamKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamKey\"\n        },\n        {\n          \"description\": \"Stream key used to authenticate an RTMPS stream for ingestion.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-create-stream-key-response-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: CreateStreamKeyResponse
---
