---
description: Required when you set (Codec) under (AudioDescriptions)>(CodecSettings) to the value AC3.
layout: schema
name: Ac3Settings
properties_list:
- description: ''
  name: Bitrate
  type: object
- description: ''
  name: BitstreamMode
  type: object
- description: ''
  name: CodingMode
  type: object
- description: ''
  name: Dialnorm
  type: object
- description: ''
  name: DynamicRangeCompressionLine
  type: object
- description: ''
  name: DynamicRangeCompressionProfile
  type: object
- description: ''
  name: DynamicRangeCompressionRf
  type: object
- description: ''
  name: LfeFilter
  type: object
- description: ''
  name: MetadataControl
  type: object
- description: ''
  name: SampleRate
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-ac3-settings-schema.json
slug: mediaconvert-api-ac3-settings
source_filename: mediaconvert-api-ac3-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-ac3-settings-schema.json\",\n  \"title\": \"Ac3Settings\",\n  \"description\": \"Required when you set (Codec) under (AudioDescriptions)>(CodecSettings) to the value AC3.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Bitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin64000Max640000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bitrate\"\n          },\n          \"description\": \"Specify the average bitrate in bits per second. The bitrate that you specify must be a multiple of 8000 within the allowed minimum and maximum values. Leave blank to use the default bitrate for the coding mode you select according ETSI TS 102 366. Valid bitrates for coding mode 1/0: Default: 96000. Minimum: 64000. Maximum:\
  \ 128000. Valid bitrates for coding mode 1/1: Default: 192000. Minimum: 128000. Maximum: 384000. Valid bitrates for coding mode 2/0: Default: 192000. Minimum: 128000. Maximum: 384000. Valid bitrates for coding mode 3/2 with FLE: Default: 384000. Minimum: 384000. Maximum: 640000.\"\n        }\n      ]\n    },\n    \"BitstreamMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ac3BitstreamMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bitstreamMode\"\n          },\n          \"description\": \"Specify the bitstream mode for the AC-3 stream that the encoder emits. For more information about the AC3 bitstream mode, see ATSC A/52-2012 (Annex E).\"\n        }\n      ]\n    },\n    \"CodingMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ac3CodingMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"codingMode\"\n          },\n          \"description\": \"Dolby Digital coding\
  \ mode. Determines number of channels.\"\n        }\n      ]\n    },\n    \"Dialnorm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max31\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dialnorm\"\n          },\n          \"description\": \"Sets the dialnorm for the output. If blank and input audio is Dolby Digital, dialnorm will be passed through.\"\n        }\n      ]\n    },\n    \"DynamicRangeCompressionLine\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ac3DynamicRangeCompressionLine\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dynamicRangeCompressionLine\"\n          },\n          \"description\": \"Choose the Dolby Digital dynamic range control (DRC) profile that MediaConvert uses when encoding the metadata in the Dolby Digital stream for the line operating mode. Related setting: When you use this setting, MediaConvert ignores any value you provide for\
  \ Dynamic range compression profile (DynamicRangeCompressionProfile). For information about the Dolby Digital DRC operating modes and profiles, see the Dynamic Range Control chapter of the Dolby Metadata Guide at https://developer.dolby.com/globalassets/professional/documents/dolby-metadata-guide.pdf.\"\n        }\n      ]\n    },\n    \"DynamicRangeCompressionProfile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ac3DynamicRangeCompressionProfile\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dynamicRangeCompressionProfile\"\n          },\n          \"description\": \"When you want to add Dolby dynamic range compression (DRC) signaling to your output stream, we recommend that you use the mode-specific settings instead of Dynamic range compression profile (DynamicRangeCompressionProfile). The mode-specific settings are Dynamic range compression profile, line mode (dynamicRangeCompressionLine) and Dynamic range compression profile,\
  \ RF mode (dynamicRangeCompressionRf). Note that when you specify values for all three settings, MediaConvert ignores the value of this setting in favor of the mode-specific settings. If you do use this setting instead of the mode-specific settings, choose None (NONE) to leave out DRC signaling. Keep the default Film standard (FILM_STANDARD) to set the profile to Dolby's film standard profile for all operating modes.\"\n        }\n      ]\n    },\n    \"DynamicRangeCompressionRf\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ac3DynamicRangeCompressionRf\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dynamicRangeCompressionRf\"\n          },\n          \"description\": \"Choose the Dolby Digital dynamic range control (DRC) profile that MediaConvert uses when encoding the metadata in the Dolby Digital stream for the RF operating mode. Related setting: When you use this setting, MediaConvert ignores any value you provide for Dynamic\
  \ range compression profile (DynamicRangeCompressionProfile). For information about the Dolby Digital DRC operating modes and profiles, see the Dynamic Range Control chapter of the Dolby Metadata Guide at https://developer.dolby.com/globalassets/professional/documents/dolby-metadata-guide.pdf.\"\n        }\n      ]\n    },\n    \"LfeFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ac3LfeFilter\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"lfeFilter\"\n          },\n          \"description\": \"Applies a 120Hz lowpass filter to the LFE channel prior to encoding. Only valid with 3_2_LFE coding mode.\"\n        }\n      ]\n    },\n    \"MetadataControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ac3MetadataControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"metadataControl\"\n          },\n          \"description\": \"When set to FOLLOW_INPUT, encoder metadata will\
  \ be sourced from the DD, DD+, or DolbyE decoder that supplied this audio data. If audio was not supplied from one of these streams, then the static metadata settings will be used.\"\n        }\n      ]\n    },\n    \"SampleRate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin48000Max48000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sampleRate\"\n          },\n          \"description\": \"This value is always 48000. It represents the sample rate in Hz.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-ac3-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Ac3Settings
---
