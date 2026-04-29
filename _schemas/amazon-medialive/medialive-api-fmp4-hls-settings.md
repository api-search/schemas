---
description: Fmp4 Hls Settings
layout: schema
name: Fmp4HlsSettings
properties_list:
- description: ''
  name: AudioRenditionSets
  type: object
- description: ''
  name: NielsenId3Behavior
  type: object
- description: ''
  name: TimedMetadataBehavior
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-fmp4-hls-settings-schema.json
slug: medialive-api-fmp4-hls-settings
source_filename: medialive-api-fmp4-hls-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-fmp4-hls-settings-schema.json\",\n  \"title\": \"Fmp4HlsSettings\",\n  \"description\": \"Fmp4 Hls Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AudioRenditionSets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioRenditionSets\"\n          },\n          \"description\": \"List all the audio groups that are used with the video output stream. Input all the audio GROUP-IDs that are associated to the video, separate by ','.\"\n        }\n      ]\n    },\n    \"NielsenId3Behavior\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Fmp4NielsenId3Behavior\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nielsenId3Behavior\"\
  \n          },\n          \"description\": \"If set to passthrough, Nielsen inaudible tones for media tracking will be detected in the input audio and an equivalent ID3 tag will be inserted in the output.\"\n        }\n      ]\n    },\n    \"TimedMetadataBehavior\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Fmp4TimedMetadataBehavior\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timedMetadataBehavior\"\n          },\n          \"description\": \"When set to passthrough, timed metadata is passed through from input to output.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-fmp4-hls-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Fmp4HlsSettings
---
