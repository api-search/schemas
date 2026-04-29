---
description: Object specifying the ingest configuration set up by the broadcaster, usually in an encoder.
layout: schema
name: IngestConfiguration
properties_list:
- description: ''
  name: audio
  type: object
- description: ''
  name: video
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-ingest-configuration-schema.json
slug: ivs-ingest-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-ingest-configuration-schema.json\",\n  \"title\": \"IngestConfiguration\",\n  \"description\": \"Object specifying the ingest configuration set up by the broadcaster, usually in an encoder.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"audio\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioConfiguration\"\n        },\n        {\n          \"description\": \"Encoder settings for audio.\"\n        }\n      ]\n    },\n    \"video\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VideoConfiguration\"\n        },\n        {\n          \"description\": \"Encoder settings for video.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-ingest-configuration-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: IngestConfiguration
---
