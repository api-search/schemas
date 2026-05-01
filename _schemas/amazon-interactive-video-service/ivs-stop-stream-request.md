---
description: StopStreamRequest schema
layout: schema
name: StopStreamRequest
properties_list:
- description: ''
  name: channelArn
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-stop-stream-request-schema.json
slug: ivs-stop-stream-request
source_filename: ivs-stop-stream-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-stop-stream-request-schema.json\",\n  \"title\": \"StopStreamRequest\",\n  \"description\": \"StopStreamRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"channelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChannelArn\"\n        },\n        {\n          \"description\": \"ARN of the channel for which the stream is to be stopped.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"channelArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-stop-stream-request-schema.json
tags:
- Live Streaming
- Media
- Video
- Real-Time
title: StopStreamRequest
---
