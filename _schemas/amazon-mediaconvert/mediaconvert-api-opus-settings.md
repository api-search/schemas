---
description: Required when you set Codec, under AudioDescriptions>CodecSettings, to the value OPUS.
layout: schema
name: OpusSettings
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
schema_file: json-schema/mediaconvert-api-opus-settings-schema.json
slug: mediaconvert-api-opus-settings
source_filename: mediaconvert-api-opus-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-opus-settings-schema.json\",\n  \"title\": \"OpusSettings\",\n  \"description\": \"Required when you set Codec, under AudioDescriptions>CodecSettings, to the value OPUS.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Bitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin32000Max192000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bitrate\"\n          },\n          \"description\": \"Optional. Specify the average bitrate in bits per second. Valid values are multiples of 8000, from 32000 through 192000. The default value is 96000, which we recommend for quality and bandwidth.\"\n        }\n      ]\n    },\n    \"Channels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"channels\"\n          },\n          \"description\": \"Specify the number of channels in this output audio track. Choosing Mono on the console gives you 1 output channel; choosing Stereo gives you 2. In the API, valid values are 1 and 2.\"\n        }\n      ]\n    },\n    \"SampleRate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin16000Max48000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sampleRate\"\n          },\n          \"description\": \"Optional. Sample rate in hz. Valid values are 16000, 24000, and 48000. The default value is 48000.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-opus-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: OpusSettings
---
