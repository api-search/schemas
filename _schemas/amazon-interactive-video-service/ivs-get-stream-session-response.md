---
description: GetStreamSessionResponse schema
layout: schema
name: GetStreamSessionResponse
properties_list:
- description: ''
  name: streamSession
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-get-stream-session-response-schema.json
slug: ivs-get-stream-session-response
source_filename: ivs-get-stream-session-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-get-stream-session-response-schema.json\",\n  \"title\": \"GetStreamSessionResponse\",\n  \"description\": \"GetStreamSessionResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"streamSession\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamSession\"\n        },\n        {\n          \"description\": \"List of stream details.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-get-stream-session-response-schema.json
tags:
- Live Streaming
- Media
- Video
- Real-Time
title: GetStreamSessionResponse
---
