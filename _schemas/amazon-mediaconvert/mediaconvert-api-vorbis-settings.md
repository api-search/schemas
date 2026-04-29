---
description: Required when you set Codec, under AudioDescriptions>CodecSettings, to the value Vorbis.
layout: schema
name: VorbisSettings
properties_list:
- description: ''
  name: Channels
  type: object
- description: ''
  name: SampleRate
  type: object
- description: ''
  name: VbrQuality
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-vorbis-settings-schema.json
slug: mediaconvert-api-vorbis-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-vorbis-settings-schema.json\",\n  \"title\": \"VorbisSettings\",\n  \"description\": \"Required when you set Codec, under AudioDescriptions>CodecSettings, to the value Vorbis.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Channels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"channels\"\n          },\n          \"description\": \"Optional. Specify the number of channels in this output audio track. Choosing Mono on the console gives you 1 output channel; choosing Stereo gives you 2. In the API, valid values are 1 and 2. The default value is 2.\"\n        }\n      ]\n    },\n    \"SampleRate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin22050Max48000\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"sampleRate\"\n          },\n          \"description\": \"Optional. Specify the audio sample rate in Hz. Valid values are 22050, 32000, 44100, and 48000. The default value is 48000.\"\n        }\n      ]\n    },\n    \"VbrQuality\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMinNegative1Max10\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"vbrQuality\"\n          },\n          \"description\": \"Optional. Specify the variable audio quality of this Vorbis output from -1 (lowest quality, ~45 kbit/s) to 10 (highest quality, ~500 kbit/s). The default value is 4 (~128 kbit/s). Values 5 and 6 are approximately 160 and 192 kbit/s, respectively.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-vorbis-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: VorbisSettings
---
