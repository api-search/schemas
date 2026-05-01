---
description: Object specifying a stream’s video configuration, as set up by the broadcaster (usually in an encoder). This is part of the <a>IngestConfiguration</a> object and used for monitoring stream health.
layout: schema
name: VideoConfiguration
properties_list:
- description: ''
  name: avcLevel
  type: object
- description: ''
  name: avcProfile
  type: object
- description: ''
  name: codec
  type: object
- description: ''
  name: encoder
  type: object
- description: ''
  name: targetBitrate
  type: object
- description: ''
  name: targetFramerate
  type: object
- description: ''
  name: videoHeight
  type: object
- description: ''
  name: videoWidth
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-video-configuration-schema.json
slug: ivs-video-configuration
source_filename: ivs-video-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-video-configuration-schema.json\",\n  \"title\": \"VideoConfiguration\",\n  \"description\": \"Object specifying a stream\\u2019s video configuration, as set up by the broadcaster (usually in an encoder). This is part of the <a>IngestConfiguration</a> object and used for monitoring stream health.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"avcLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Indicates the degree of required decoder performance for a profile. Normally this is set automatically by the encoder. For details, see the H.264 specification.\"\n        }\n      ]\n    },\n    \"avcProfile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\
  \n        },\n        {\n          \"description\": \"Indicates to the decoder the requirements for decoding the stream. For definitions of the valid values, see the H.264 specification.\"\n        }\n      ]\n    },\n    \"codec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Codec used for the video encoding.\"\n        }\n      ]\n    },\n    \"encoder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Software or hardware used to encode the video.\"\n        }\n      ]\n    },\n    \"targetBitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The expected ingest bitrate (bits per second). This is configured in the encoder.\"\n        }\n      ]\n    },\n    \"targetFramerate\": {\n      \"allOf\": [\n   \
  \     {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The expected ingest framerate. This is configured in the encoder.\"\n        }\n      ]\n    },\n    \"videoHeight\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"Video-resolution height in pixels.\"\n        }\n      ]\n    },\n    \"videoWidth\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"Video-resolution width in pixels.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-video-configuration-schema.json
tags:
- Live Streaming
- Media
- Video
- Real-Time
title: VideoConfiguration
---
