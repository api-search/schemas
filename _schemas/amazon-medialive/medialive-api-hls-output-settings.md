---
description: Hls Output Settings
layout: schema
name: HlsOutputSettings
properties_list:
- description: ''
  name: H265PackagingType
  type: object
- description: ''
  name: HlsSettings
  type: object
- description: ''
  name: NameModifier
  type: object
- description: ''
  name: SegmentModifier
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-hls-output-settings-schema.json
slug: medialive-api-hls-output-settings
source_filename: medialive-api-hls-output-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-hls-output-settings-schema.json\",\n  \"title\": \"HlsOutputSettings\",\n  \"description\": \"Hls Output Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"H265PackagingType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsH265PackagingType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"h265PackagingType\"\n          },\n          \"description\": \"Only applicable when this output is referencing an H.265 video description.\\nSpecifies whether MP4 segments should be packaged as HEV1 or HVC1.\"\n        }\n      ]\n    },\n    \"HlsSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hlsSettings\"\n\
  \          },\n          \"description\": \"Settings regarding the underlying stream. These settings are different for audio-only outputs.\"\n        }\n      ]\n    },\n    \"NameModifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nameModifier\"\n          },\n          \"description\": \"String concatenated to the end of the destination filename. Accepts \\\\\\\"Format Identifiers\\\\\\\":#formatIdentifierParameters.\"\n        }\n      ]\n    },\n    \"SegmentModifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentModifier\"\n          },\n          \"description\": \"String concatenated to end of segment filenames.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"HlsSettings\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-hls-output-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: HlsOutputSettings
---
