---
description: GetPlaybackKeyPairRequest schema
layout: schema
name: GetPlaybackKeyPairRequest
properties_list:
- description: ''
  name: arn
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-get-playback-key-pair-request-schema.json
slug: ivs-get-playback-key-pair-request
source_filename: ivs-get-playback-key-pair-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-get-playback-key-pair-request-schema.json\",\n  \"title\": \"GetPlaybackKeyPairRequest\",\n  \"description\": \"GetPlaybackKeyPairRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlaybackKeyPairArn\"\n        },\n        {\n          \"description\": \"ARN of the key pair to be returned.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-get-playback-key-pair-request-schema.json
tags:
- Live Streaming
- Media
- Video
- Real-Time
title: GetPlaybackKeyPairRequest
---
