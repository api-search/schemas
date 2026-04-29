---
description: BatchGetChannelRequest schema
layout: schema
name: BatchGetChannelRequest
properties_list:
- description: ''
  name: arns
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-batch-get-channel-request-schema.json
slug: ivs-batch-get-channel-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-batch-get-channel-request-schema.json\",\n  \"title\": \"BatchGetChannelRequest\",\n  \"description\": \"BatchGetChannelRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChannelArnList\"\n        },\n        {\n          \"description\": \"Array of ARNs, one per channel.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arns\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-batch-get-channel-request-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: BatchGetChannelRequest
---
