---
description: ListPlaybackKeyPairsRequest schema
layout: schema
name: ListPlaybackKeyPairsRequest
properties_list:
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-list-playback-key-pairs-request-schema.json
slug: ivs-list-playback-key-pairs-request
source_filename: ivs-list-playback-key-pairs-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-list-playback-key-pairs-request-schema.json\",\n  \"title\": \"ListPlaybackKeyPairsRequest\",\n  \"description\": \"ListPlaybackKeyPairsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxPlaybackKeyPairResults\"\n        },\n        {\n          \"description\": \"Maximum number of key pairs to return. Default: your service quota or 100, whichever is smaller.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The first key pair to retrieve. This is used for pagination; see the <code>nextToken</code> response field.\"\n      \
  \  }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-list-playback-key-pairs-request-schema.json
tags:
- Live Streaming
- Media
- Video
- Real-Time
title: ListPlaybackKeyPairsRequest
---
