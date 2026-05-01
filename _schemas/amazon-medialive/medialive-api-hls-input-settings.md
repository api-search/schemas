---
description: Hls Input Settings
layout: schema
name: HlsInputSettings
properties_list:
- description: ''
  name: Bandwidth
  type: object
- description: ''
  name: BufferSegments
  type: object
- description: ''
  name: Retries
  type: object
- description: ''
  name: RetryInterval
  type: object
- description: ''
  name: Scte35Source
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-hls-input-settings-schema.json
slug: medialive-api-hls-input-settings
source_filename: medialive-api-hls-input-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-hls-input-settings-schema.json\",\n  \"title\": \"HlsInputSettings\",\n  \"description\": \"Hls Input Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Bandwidth\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bandwidth\"\n          },\n          \"description\": \"When specified the HLS stream with the m3u8 BANDWIDTH that most closely matches this value will be chosen, otherwise the highest bandwidth stream in the m3u8 will be chosen.  The bitrate is specified in bits per second, as in an HLS manifest.\"\n        }\n      ]\n    },\n    \"BufferSegments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n      \
  \  },\n        {\n          \"xml\": {\n            \"name\": \"bufferSegments\"\n          },\n          \"description\": \"When specified, reading of the HLS input will begin this many buffer segments from the end (most recently written segment).  When not specified, the HLS input will begin with the first segment specified in the m3u8.\"\n        }\n      ]\n    },\n    \"Retries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"retries\"\n          },\n          \"description\": \"The number of consecutive times that attempts to read a manifest or segment must fail before the input is considered unavailable.\"\n        }\n      ]\n    },\n    \"RetryInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"retryInterval\"\n          },\n          \"description\"\
  : \"The number of seconds between retries when an attempt to read a manifest or segment fails.\"\n        }\n      ]\n    },\n    \"Scte35Source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsScte35SourceType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scte35Source\"\n          },\n          \"description\": \"Identifies the source for the SCTE-35 messages that MediaLive will ingest. Messages can be ingested from the content segments (in the stream) or from tags in the playlist (the HLS manifest). MediaLive ignores SCTE-35 information in the source that is not selected.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-hls-input-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: HlsInputSettings
---
