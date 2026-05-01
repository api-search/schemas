---
description: GetPlaybackKeyPairResponse schema
layout: schema
name: GetPlaybackKeyPairResponse
properties_list:
- description: ''
  name: keyPair
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-get-playback-key-pair-response-schema.json
slug: ivs-get-playback-key-pair-response
source_filename: ivs-get-playback-key-pair-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-get-playback-key-pair-response-schema.json\",\n  \"title\": \"GetPlaybackKeyPairResponse\",\n  \"description\": \"GetPlaybackKeyPairResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"keyPair\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlaybackKeyPair\"\n        },\n        {\n          \"description\": \"<zonbook></zonbook><xhtml></xhtml>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-get-playback-key-pair-response-schema.json
tags:
- Live Streaming
- Media
- Video
- Real-Time
title: GetPlaybackKeyPairResponse
---
