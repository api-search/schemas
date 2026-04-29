---
description: CreateStreamKeyRequest schema
layout: schema
name: CreateStreamKeyRequest
properties_list:
- description: ''
  name: channelArn
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-create-stream-key-request-schema.json
slug: ivs-create-stream-key-request
source_filename: ivs-create-stream-key-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-create-stream-key-request-schema.json\",\n  \"title\": \"CreateStreamKeyRequest\",\n  \"description\": \"CreateStreamKeyRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"channelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChannelArn\"\n        },\n        {\n          \"description\": \"ARN of the channel for which to create the stream key.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"Array of 1-50 maps, each of the form <code>string:string (key:value)</code>. See <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\\\">Tagging Amazon Web Services Resources</a> for more\
  \ information, including restrictions that apply to tags and \\\"Tag naming limits and requirements\\\"; Amazon IVS has no service-specific constraints beyond what is documented there.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"channelArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-create-stream-key-request-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: CreateStreamKeyRequest
---
