---
description: Required when you set (Codec) under (AudioDescriptions)>(CodecSettings) to the value EAC3_ATMOS.
layout: schema
name: Eac3AtmosSettings
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
  name: DialogueIntelligence
  type: object
- description: ''
  name: DownmixControl
  type: object
- description: ''
  name: DynamicRangeCompressionLine
  type: object
- description: ''
  name: DynamicRangeCompressionRf
  type: object
- description: ''
  name: DynamicRangeControl
  type: object
- description: ''
  name: LoRoCenterMixLevel
  type: object
- description: ''
  name: LoRoSurroundMixLevel
  type: object
- description: ''
  name: LtRtCenterMixLevel
  type: object
- description: ''
  name: LtRtSurroundMixLevel
  type: object
- description: ''
  name: MeteringMode
  type: object
- description: ''
  name: SampleRate
  type: object
- description: ''
  name: SpeechThreshold
  type: object
- description: ''
  name: StereoDownmix
  type: object
- description: ''
  name: SurroundExMode
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-eac3-atmos-settings-schema.json
slug: mediaconvert-api-eac3-atmos-settings
source_filename: mediaconvert-api-eac3-atmos-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-eac3-atmos-settings-schema.json\",\n  \"title\": \"Eac3AtmosSettings\",\n  \"description\": \"Required when you set (Codec) under (AudioDescriptions)>(CodecSettings) to the value EAC3_ATMOS.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Bitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin384000Max1024000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bitrate\"\n          },\n          \"description\": \"Specify the average bitrate for this output in bits per second. Valid values: 384k, 448k, 576k, 640k, 768k, 1024k Default value: 448k Note that MediaConvert supports 384k only with channel-based immersive (CBI) 7.1.4 and 5.1.4 inputs. For CBI 9.1.6 and other input types, MediaConvert automatically increases\
  \ your output bitrate to 448k.\"\n        }\n      ]\n    },\n    \"BitstreamMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3AtmosBitstreamMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bitstreamMode\"\n          },\n          \"description\": \"Specify the bitstream mode for the E-AC-3 stream that the encoder emits. For more information about the EAC3 bitstream mode, see ATSC A/52-2012 (Annex E).\"\n        }\n      ]\n    },\n    \"CodingMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3AtmosCodingMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"codingMode\"\n          },\n          \"description\": \"The coding mode for Dolby Digital Plus JOC (Atmos).\"\n        }\n      ]\n    },\n    \"DialogueIntelligence\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3AtmosDialogueIntelligence\"\n        },\n        {\n    \
  \      \"xml\": {\n            \"name\": \"dialogueIntelligence\"\n          },\n          \"description\": \"Enable Dolby Dialogue Intelligence to adjust loudness based on dialogue analysis.\"\n        }\n      ]\n    },\n    \"DownmixControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3AtmosDownmixControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"downmixControl\"\n          },\n          \"description\": \"Specify whether MediaConvert should use any downmix metadata from your input file. Keep the default value, Custom (SPECIFIED) to provide downmix values in your job settings. Choose Follow source (INITIALIZE_FROM_SOURCE) to use the metadata from your input. Related settings--Use these settings to specify your downmix values: Left only/Right only surround (LoRoSurroundMixLevel), Left total/Right total surround (LtRtSurroundMixLevel), Left total/Right total center (LtRtCenterMixLevel), Left only/Right only center (LoRoCenterMixLevel),\
  \ and Stereo downmix (StereoDownmix). When you keep Custom (SPECIFIED) for Downmix control (DownmixControl) and you don't specify values for the related settings, MediaConvert uses default values for those settings.\"\n        }\n      ]\n    },\n    \"DynamicRangeCompressionLine\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3AtmosDynamicRangeCompressionLine\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dynamicRangeCompressionLine\"\n          },\n          \"description\": \"Choose the Dolby dynamic range control (DRC) profile that MediaConvert uses when encoding the metadata in the Dolby stream for the line operating mode. Default value: Film light (ATMOS_STORAGE_DDP_COMPR_FILM_LIGHT) Related setting: To have MediaConvert use the value you specify here, keep the default value, Custom (SPECIFIED) for the setting Dynamic range control (DynamicRangeControl). Otherwise, MediaConvert ignores Dynamic range compression line (DynamicRangeCompressionLine).\
  \ For information about the Dolby DRC operating modes and profiles, see the Dynamic Range Control chapter of the Dolby Metadata Guide at https://developer.dolby.com/globalassets/professional/documents/dolby-metadata-guide.pdf.\"\n        }\n      ]\n    },\n    \"DynamicRangeCompressionRf\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3AtmosDynamicRangeCompressionRf\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dynamicRangeCompressionRf\"\n          },\n          \"description\": \"Choose the Dolby dynamic range control (DRC) profile that MediaConvert uses when encoding the metadata in the Dolby stream for the RF operating mode. Default value: Film light (ATMOS_STORAGE_DDP_COMPR_FILM_LIGHT) Related setting: To have MediaConvert use the value you specify here, keep the default value, Custom (SPECIFIED) for the setting Dynamic range control (DynamicRangeControl). Otherwise, MediaConvert ignores Dynamic range compression RF (DynamicRangeCompressionRf).\
  \ For information about the Dolby DRC operating modes and profiles, see the Dynamic Range Control chapter of the Dolby Metadata Guide at https://developer.dolby.com/globalassets/professional/documents/dolby-metadata-guide.pdf.\"\n        }\n      ]\n    },\n    \"DynamicRangeControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3AtmosDynamicRangeControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dynamicRangeControl\"\n          },\n          \"description\": \"Specify whether MediaConvert should use any dynamic range control metadata from your input file. Keep the default value, Custom (SPECIFIED), to provide dynamic range control values in your job settings. Choose Follow source (INITIALIZE_FROM_SOURCE) to use the metadata from your input. Related settings--Use these settings to specify your dynamic range control values: Dynamic range compression line (DynamicRangeCompressionLine) and Dynamic range compression RF (DynamicRangeCompressionRf).\
  \ When you keep the value Custom (SPECIFIED) for Dynamic range control (DynamicRangeControl) and you don't specify values for the related settings, MediaConvert uses default values for those settings.\"\n        }\n      ]\n    },\n    \"LoRoCenterMixLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMinNegative6Max3\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"loRoCenterMixLevel\"\n          },\n          \"description\": \"Specify a value for the following Dolby Atmos setting: Left only/Right only center mix (Lo/Ro center). MediaConvert uses this value for downmixing. Default value: -3 dB (ATMOS_STORAGE_DDP_MIXLEV_MINUS_3_DB). Valid values: 3.0, 1.5, 0.0, -1.5, -3.0, -4.5, and -6.0. Related setting: How the service uses this value depends on the value that you choose for Stereo downmix (Eac3AtmosStereoDownmix). Related setting: To have MediaConvert use this value, keep the default value, Custom (SPECIFIED) for the\
  \ setting Downmix control (DownmixControl). Otherwise, MediaConvert ignores Left only/Right only center (LoRoCenterMixLevel).\"\n        }\n      ]\n    },\n    \"LoRoSurroundMixLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMinNegative60MaxNegative1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"loRoSurroundMixLevel\"\n          },\n          \"description\": \"Specify a value for the following Dolby Atmos setting: Left only/Right only (Lo/Ro surround). MediaConvert uses this value for downmixing. Default value: -3 dB (ATMOS_STORAGE_DDP_MIXLEV_MINUS_3_DB). Valid values: -1.5, -3.0, -4.5, -6.0, and -60. The value -60 mutes the channel. Related setting: How the service uses this value depends on the value that you choose for Stereo downmix (Eac3AtmosStereoDownmix). Related setting: To have MediaConvert use this value, keep the default value, Custom (SPECIFIED) for the setting Downmix control (DownmixControl). Otherwise,\
  \ MediaConvert ignores Left only/Right only surround (LoRoSurroundMixLevel).\"\n        }\n      ]\n    },\n    \"LtRtCenterMixLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMinNegative6Max3\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ltRtCenterMixLevel\"\n          },\n          \"description\": \"Specify a value for the following Dolby Atmos setting: Left total/Right total center mix (Lt/Rt center). MediaConvert uses this value for downmixing. Default value: -3 dB (ATMOS_STORAGE_DDP_MIXLEV_MINUS_3_DB) Valid values: 3.0, 1.5, 0.0, -1.5, -3.0, -4.5, and -6.0. Related setting: How the service uses this value depends on the value that you choose for Stereo downmix (Eac3AtmosStereoDownmix). Related setting: To have MediaConvert use this value, keep the default value, Custom (SPECIFIED) for the setting Downmix control (DownmixControl). Otherwise, MediaConvert ignores Left total/Right total center (LtRtCenterMixLevel).\"\
  \n        }\n      ]\n    },\n    \"LtRtSurroundMixLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMinNegative60MaxNegative1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ltRtSurroundMixLevel\"\n          },\n          \"description\": \"Specify a value for the following Dolby Atmos setting: Left total/Right total surround mix (Lt/Rt surround). MediaConvert uses this value for downmixing. Default value: -3 dB (ATMOS_STORAGE_DDP_MIXLEV_MINUS_3_DB) Valid values: -1.5, -3.0, -4.5, -6.0, and -60. The value -60 mutes the channel. Related setting: How the service uses this value depends on the value that you choose for Stereo downmix (Eac3AtmosStereoDownmix). Related setting: To have MediaConvert use this value, keep the default value, Custom (SPECIFIED) for the setting Downmix control (DownmixControl). Otherwise, the service ignores Left total/Right total surround (LtRtSurroundMixLevel).\"\n        }\n      ]\n    },\n\
  \    \"MeteringMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3AtmosMeteringMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"meteringMode\"\n          },\n          \"description\": \"Choose how the service meters the loudness of your audio.\"\n        }\n      ]\n    },\n    \"SampleRate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin48000Max48000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sampleRate\"\n          },\n          \"description\": \"This value is always 48000. It represents the sample rate in Hz.\"\n        }\n      ]\n    },\n    \"SpeechThreshold\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max100\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"speechThreshold\"\n          },\n          \"description\": \"Specify the percentage of audio content, from 0% to 100%,\
  \ that must be speech in order for the encoder to use the measured speech loudness as the overall program loudness. Default value: 15%\"\n        }\n      ]\n    },\n    \"StereoDownmix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3AtmosStereoDownmix\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"stereoDownmix\"\n          },\n          \"description\": \"Choose how the service does stereo downmixing. Default value: Not indicated (ATMOS_STORAGE_DDP_DMIXMOD_NOT_INDICATED) Related setting: To have MediaConvert use this value, keep the default value, Custom (SPECIFIED) for the setting Downmix control (DownmixControl). Otherwise, MediaConvert ignores Stereo downmix (StereoDownmix).\"\n        }\n      ]\n    },\n    \"SurroundExMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3AtmosSurroundExMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"surroundExMode\"\n   \
  \       },\n          \"description\": \"Specify whether your input audio has an additional center rear surround channel matrix encoded into your left and right surround channels.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-eac3-atmos-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Eac3AtmosSettings
---
