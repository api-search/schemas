---
description: Mp2 Settings
layout: schema
name: Mp2Settings
properties_list:
- description: ''
  name: Bitrate
  type: object
- description: ''
  name: CodingMode
  type: object
- description: ''
  name: SampleRate
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-mp2-settings-schema.json
slug: medialive-api-mp2-settings
source_filename: medialive-api-mp2-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-mp2-settings-schema.json\",\n  \"title\": \"Mp2Settings\",\n  \"description\": \"Mp2 Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Bitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bitrate\"\n          },\n          \"description\": \"Average bitrate in bits/second.\"\n        }\n      ]\n    },\n    \"CodingMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mp2CodingMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"codingMode\"\n          },\n          \"description\": \"The MPEG2 Audio coding mode.  Valid values are codingMode10 (for mono) or codingMode20 (for stereo).\"\n        }\n      ]\n\
  \    },\n    \"SampleRate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sampleRate\"\n          },\n          \"description\": \"Sample rate in Hz.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-mp2-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Mp2Settings
---
