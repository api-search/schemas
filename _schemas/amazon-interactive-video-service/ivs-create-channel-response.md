---
description: CreateChannelResponse schema
layout: schema
name: CreateChannelResponse
properties_list:
- description: ''
  name: channel
  type: object
- description: ''
  name: streamKey
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-create-channel-response-schema.json
slug: ivs-create-channel-response
source_filename: ivs-create-channel-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-create-channel-response-schema.json\",\n  \"title\": \"CreateChannelResponse\",\n  \"description\": \"CreateChannelResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"channel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Channel\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    },\n    \"streamKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamKey\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-create-channel-response-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: CreateChannelResponse
---
