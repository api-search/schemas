---
description: Wav Settings
layout: schema
name: WavSettings
properties_list:
- description: ''
  name: BitDepth
  type: object
- description: ''
  name: CodingMode
  type: object
- description: ''
  name: SampleRate
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-wav-settings-schema.json
slug: medialive-api-wav-settings
source_filename: medialive-api-wav-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-wav-settings-schema.json\",\n  \"title\": \"WavSettings\",\n  \"description\": \"Wav Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BitDepth\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bitDepth\"\n          },\n          \"description\": \"Bits per sample.\"\n        }\n      ]\n    },\n    \"CodingMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WavCodingMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"codingMode\"\n          },\n          \"description\": \"The audio coding mode for the WAV audio. The mode determines the number of channels in the audio.\"\n        }\n      ]\n    },\n    \"\
  SampleRate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sampleRate\"\n          },\n          \"description\": \"Sample rate in Hz.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-wav-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: WavSettings
---
