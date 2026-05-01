---
description: Required when you set (Codec) under (AudioDescriptions)>(CodecSettings) to the value WAV.
layout: schema
name: WavSettings
properties_list:
- description: ''
  name: BitDepth
  type: object
- description: ''
  name: Channels
  type: object
- description: ''
  name: Format
  type: object
- description: ''
  name: SampleRate
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-wav-settings-schema.json
slug: mediaconvert-api-wav-settings
source_filename: mediaconvert-api-wav-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-wav-settings-schema.json\",\n  \"title\": \"WavSettings\",\n  \"description\": \"Required when you set (Codec) under (AudioDescriptions)>(CodecSettings) to the value WAV.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BitDepth\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin16Max24\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bitDepth\"\n          },\n          \"description\": \"Specify Bit depth (BitDepth), in bits per sample, to choose the encoding quality for this audio track.\"\n        }\n      ]\n    },\n    \"Channels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max64\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"channels\"\
  \n          },\n          \"description\": \"Specify the number of channels in this output audio track. Valid values are 1 and even numbers up to 64. For example, 1, 2, 4, 6, and so on, up to 64.\"\n        }\n      ]\n    },\n    \"Format\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WavFormat\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"format\"\n          },\n          \"description\": \"The service defaults to using RIFF for WAV outputs. If your output audio is likely to exceed 4 GB in file size, or if you otherwise need the extended support of the RF64 format, set your output WAV file format to RF64.\"\n        }\n      ]\n    },\n    \"SampleRate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin8000Max192000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sampleRate\"\n          },\n          \"description\": \"Sample rate in Hz.\"\n        }\n      ]\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-wav-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: WavSettings
---
