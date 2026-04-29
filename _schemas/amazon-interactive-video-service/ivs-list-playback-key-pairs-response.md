---
description: ListPlaybackKeyPairsResponse schema
layout: schema
name: ListPlaybackKeyPairsResponse
properties_list:
- description: ''
  name: keyPairs
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-list-playback-key-pairs-response-schema.json
slug: ivs-list-playback-key-pairs-response
source_filename: ivs-list-playback-key-pairs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-list-playback-key-pairs-response-schema.json\",\n  \"title\": \"ListPlaybackKeyPairsResponse\",\n  \"description\": \"ListPlaybackKeyPairsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"keyPairs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlaybackKeyPairList\"\n        },\n        {\n          \"description\": \"List of key pairs.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"If there are more key pairs than <code>maxResults</code>, use <code>nextToken</code> in the request to get the next set.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"keyPairs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-list-playback-key-pairs-response-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: ListPlaybackKeyPairsResponse
---
