---
description: PutMetadataRequest schema
layout: schema
name: PutMetadataRequest
properties_list:
- description: ''
  name: channelArn
  type: object
- description: ''
  name: metadata
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-put-metadata-request-schema.json
slug: ivs-put-metadata-request
source_filename: ivs-put-metadata-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-put-metadata-request-schema.json\",\n  \"title\": \"PutMetadataRequest\",\n  \"description\": \"PutMetadataRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"channelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChannelArn\"\n        },\n        {\n          \"description\": \"ARN of the channel into which metadata is inserted. This channel must have an active stream.\"\n        }\n      ]\n    },\n    \"metadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamMetadata\"\n        },\n        {\n          \"description\": \"Metadata to insert into the stream. Maximum: 1 KB per request.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"channelArn\",\n    \"metadata\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-put-metadata-request-schema.json
tags:
- Live Streaming
- Media
- Video
- Real-Time
title: PutMetadataRequest
---
