---
description: Object specifying a stream’s audio configuration, as set up by the broadcaster (usually in an encoder). This is part of the <a>IngestConfiguration</a> object and used for monitoring stream health.
layout: schema
name: AudioConfiguration
properties_list:
- description: ''
  name: channels
  type: object
- description: ''
  name: codec
  type: object
- description: ''
  name: sampleRate
  type: object
- description: ''
  name: targetBitrate
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-audio-configuration-schema.json
slug: ivs-audio-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-audio-configuration-schema.json\",\n  \"title\": \"AudioConfiguration\",\n  \"description\": \"Object specifying a stream\\u2019s audio configuration, as set up by the broadcaster (usually in an encoder). This is part of the <a>IngestConfiguration</a> object and used for monitoring stream health.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"channels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"Number of audio channels.\"\n        }\n      ]\n    },\n    \"codec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Codec used for the audio encoding.\"\n        }\n      ]\n    },\n    \"sampleRate\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"Number of audio samples recorded per second.\"\n        }\n      ]\n    },\n    \"targetBitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The expected ingest bitrate (bits per second). This is configured in the encoder.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-audio-configuration-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: AudioConfiguration
---
