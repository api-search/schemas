---
description: ImportPlaybackKeyPairResponse schema
layout: schema
name: ImportPlaybackKeyPairResponse
properties_list:
- description: ''
  name: keyPair
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-import-playback-key-pair-response-schema.json
slug: ivs-import-playback-key-pair-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-import-playback-key-pair-response-schema.json\",\n  \"title\": \"ImportPlaybackKeyPairResponse\",\n  \"description\": \"ImportPlaybackKeyPairResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"keyPair\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlaybackKeyPair\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-import-playback-key-pair-response-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: ImportPlaybackKeyPairResponse
---
