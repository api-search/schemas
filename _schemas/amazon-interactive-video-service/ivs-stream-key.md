---
description: Object specifying a stream key.
layout: schema
name: StreamKey
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: channelArn
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: value
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-stream-key-schema.json
slug: ivs-stream-key
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-stream-key-schema.json\",\n  \"title\": \"StreamKey\",\n  \"description\": \"Object specifying a stream key.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamKeyArn\"\n        },\n        {\n          \"description\": \"Stream-key ARN.\"\n        }\n      ]\n    },\n    \"channelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChannelArn\"\n        },\n        {\n          \"description\": \"Channel ARN for the stream.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"Tags attached to the resource. Array of 1-50 maps, each\
  \ of the form <code>string:string (key:value)</code>. See <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\\\">Tagging Amazon Web Services Resources</a> for more information, including restrictions that apply to tags and \\\"Tag naming limits and requirements\\\"; Amazon IVS has no service-specific constraints beyond what is documented there.\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamKeyValue\"\n        },\n        {\n          \"description\": \"Stream-key value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-stream-key-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: StreamKey
---
