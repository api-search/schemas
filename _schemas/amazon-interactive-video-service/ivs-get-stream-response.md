---
description: GetStreamResponse schema
layout: schema
name: GetStreamResponse
properties_list:
- description: ''
  name: stream
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-get-stream-response-schema.json
slug: ivs-get-stream-response
source_filename: ivs-get-stream-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-get-stream-response-schema.json\",\n  \"title\": \"GetStreamResponse\",\n  \"description\": \"GetStreamResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stream\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Stream\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-get-stream-response-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: GetStreamResponse
---
