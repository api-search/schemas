---
description: GetStreamSessionRequest schema
layout: schema
name: GetStreamSessionRequest
properties_list:
- description: ''
  name: channelArn
  type: object
- description: ''
  name: streamId
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-get-stream-session-request-schema.json
slug: ivs-get-stream-session-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-get-stream-session-request-schema.json\",\n  \"title\": \"GetStreamSessionRequest\",\n  \"description\": \"GetStreamSessionRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"channelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChannelArn\"\n        },\n        {\n          \"description\": \"ARN of the channel resource\"\n        }\n      ]\n    },\n    \"streamId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamId\"\n        },\n        {\n          \"description\": \"Unique identifier for a live or previously live stream in the specified channel. If no <code>streamId</code> is provided, this returns the most recent stream session for the channel, if it exists.\"\n        }\n      ]\n  \
  \  }\n  },\n  \"required\": [\n    \"channelArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-get-stream-session-request-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: GetStreamSessionRequest
---
