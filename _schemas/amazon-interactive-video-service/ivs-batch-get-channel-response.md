---
description: BatchGetChannelResponse schema
layout: schema
name: BatchGetChannelResponse
properties_list:
- description: ''
  name: channels
  type: object
- description: ''
  name: errors
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-batch-get-channel-response-schema.json
slug: ivs-batch-get-channel-response
source_filename: ivs-batch-get-channel-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-batch-get-channel-response-schema.json\",\n  \"title\": \"BatchGetChannelResponse\",\n  \"description\": \"BatchGetChannelResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"channels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Channels\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    },\n    \"errors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchErrors\"\n        },\n        {\n          \"description\": \"Each error object is related to a specific ARN in the request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-batch-get-channel-response-schema.json
tags:
- Live Streaming
- Media
- Video
- Real-Time
title: BatchGetChannelResponse
---
