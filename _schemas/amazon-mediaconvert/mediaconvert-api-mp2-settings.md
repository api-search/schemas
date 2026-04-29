---
description: Required when you set (Codec) under (AudioDescriptions)>(CodecSettings) to the value MP2.
layout: schema
name: Mp2Settings
properties_list:
- description: ''
  name: Bitrate
  type: object
- description: ''
  name: Channels
  type: object
- description: ''
  name: SampleRate
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-mp2-settings-schema.json
slug: mediaconvert-api-mp2-settings
source_filename: mediaconvert-api-mp2-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mp2-settings-schema.json\",\n  \"title\": \"Mp2Settings\",\n  \"description\": \"Required when you set (Codec) under (AudioDescriptions)>(CodecSettings) to the value MP2.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Bitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin32000Max384000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bitrate\"\n          },\n          \"description\": \"Specify the average bitrate in bits per second.\"\n        }\n      ]\n    },\n    \"Channels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"channels\"\n          },\n          \"description\": \"Set Channels\
  \ to specify the number of channels in this output audio track. Choosing Mono in the console will give you 1 output channel; choosing Stereo will give you 2. In the API, valid values are 1 and 2.\"\n        }\n      ]\n    },\n    \"SampleRate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin32000Max48000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sampleRate\"\n          },\n          \"description\": \"Sample rate in hz.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mp2-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Mp2Settings
---
