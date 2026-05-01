---
description: Required when you set Codec, under AudioDescriptions>CodecSettings, to the value MP3.
layout: schema
name: Mp3Settings
properties_list:
- description: ''
  name: Bitrate
  type: object
- description: ''
  name: Channels
  type: object
- description: ''
  name: RateControlMode
  type: object
- description: ''
  name: SampleRate
  type: object
- description: ''
  name: VbrQuality
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-mp3-settings-schema.json
slug: mediaconvert-api-mp3-settings
source_filename: mediaconvert-api-mp3-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mp3-settings-schema.json\",\n  \"title\": \"Mp3Settings\",\n  \"description\": \"Required when you set Codec, under AudioDescriptions>CodecSettings, to the value MP3.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Bitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin16000Max320000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bitrate\"\n          },\n          \"description\": \"Specify the average bitrate in bits per second.\"\n        }\n      ]\n    },\n    \"Channels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"channels\"\n          },\n          \"description\": \"Specify the\
  \ number of channels in this output audio track. Choosing Mono on the console gives you 1 output channel; choosing Stereo gives you 2. In the API, valid values are 1 and 2.\"\n        }\n      ]\n    },\n    \"RateControlMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mp3RateControlMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"rateControlMode\"\n          },\n          \"description\": \"Specify whether the service encodes this MP3 audio output with a constant bitrate (CBR) or a variable bitrate (VBR).\"\n        }\n      ]\n    },\n    \"SampleRate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin22050Max48000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sampleRate\"\n          },\n          \"description\": \"Sample rate in hz.\"\n        }\n      ]\n    },\n    \"VbrQuality\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max9\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"vbrQuality\"\n          },\n          \"description\": \"Required when you set Bitrate control mode (rateControlMode) to VBR. Specify the audio quality of this MP3 output from 0 (highest quality) to 9 (lowest quality).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mp3-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Mp3Settings
---
