---
description: Required when you set (Codec) under (AudioDescriptions)>(CodecSettings) to the value AAC. The service accepts one of two mutually exclusive groups of AAC settings--VBR and CBR. To select one of these modes, set the value of Bitrate control mode (rateControlMode) to "VBR" or "CBR". In VBR mode, you control the audio quality with the setting VBR quality (vbrQuality). In CBR mode, you use the setting Bitrate (bitrate). Defaults and valid values depend on the rate control mode.
layout: schema
name: AacSettings
properties_list:
- description: ''
  name: AudioDescriptionBroadcasterMix
  type: object
- description: ''
  name: Bitrate
  type: object
- description: ''
  name: CodecProfile
  type: object
- description: ''
  name: CodingMode
  type: object
- description: ''
  name: RateControlMode
  type: object
- description: ''
  name: RawFormat
  type: object
- description: ''
  name: SampleRate
  type: object
- description: ''
  name: Specification
  type: object
- description: ''
  name: VbrQuality
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-aac-settings-schema.json
slug: mediaconvert-api-aac-settings
source_filename: mediaconvert-api-aac-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-aac-settings-schema.json\",\n  \"title\": \"AacSettings\",\n  \"description\": \"Required when you set (Codec) under (AudioDescriptions)>(CodecSettings) to the value AAC. The service accepts one of two mutually exclusive groups of AAC settings--VBR and CBR. To select one of these modes, set the value of Bitrate control mode (rateControlMode) to \\\"VBR\\\" or \\\"CBR\\\". In VBR mode, you control the audio quality with the setting VBR quality (vbrQuality). In CBR mode, you use the setting Bitrate (bitrate). Defaults and valid values depend on the rate control mode.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AudioDescriptionBroadcasterMix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AacAudioDescriptionBroadcasterMix\"\n        },\n   \
  \     {\n          \"xml\": {\n            \"name\": \"audioDescriptionBroadcasterMix\"\n          },\n          \"description\": \"Choose BROADCASTER_MIXED_AD when the input contains pre-mixed main audio + audio description (AD) as a stereo pair. The value for AudioType will be set to 3, which signals to downstream systems that this stream contains \\\"broadcaster mixed AD\\\". Note that the input received by the encoder must contain pre-mixed audio; the encoder does not perform the mixing. When you choose BROADCASTER_MIXED_AD, the encoder ignores any values you provide in AudioType and FollowInputAudioType. Choose NORMAL when the input does not contain pre-mixed audio + audio description (AD). In this case, the encoder will use any values you provide for AudioType and FollowInputAudioType.\"\n        }\n      ]\n    },\n    \"Bitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin6000Max1024000\"\n        },\n        {\n          \"xml\":\
  \ {\n            \"name\": \"bitrate\"\n          },\n          \"description\": \"Specify the average bitrate in bits per second. The set of valid values for this setting is: 6000, 8000, 10000, 12000, 14000, 16000, 20000, 24000, 28000, 32000, 40000, 48000, 56000, 64000, 80000, 96000, 112000, 128000, 160000, 192000, 224000, 256000, 288000, 320000, 384000, 448000, 512000, 576000, 640000, 768000, 896000, 1024000. The value you set is also constrained by the values that you choose for Profile (codecProfile), Bitrate control mode (codingMode), and Sample rate (sampleRate). Default values depend on Bitrate control mode and Profile.\"\n        }\n      ]\n    },\n    \"CodecProfile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AacCodecProfile\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"codecProfile\"\n          },\n          \"description\": \"AAC Profile.\"\n        }\n      ]\n    },\n    \"CodingMode\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/AacCodingMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"codingMode\"\n          },\n          \"description\": \"The Coding mode that you specify determines the number of audio channels and the audio channel layout metadata in your AAC output. Valid coding modes depend on the Rate control mode and Profile that you select. The following list shows the number of audio channels and channel layout for each coding mode. * 1.0 Audio Description (Receiver Mix): One channel, C. Includes audio description data from your stereo input. For more information see ETSI TS 101 154 Annex E. * 1.0 Mono: One channel, C. * 2.0 Stereo: Two channels, L, R. * 5.1 Surround: Five channels, C, L, R, Ls, Rs, LFE.\"\n        }\n      ]\n    },\n    \"RateControlMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AacRateControlMode\"\n        },\n        {\n          \"xml\": {\n            \"name\"\
  : \"rateControlMode\"\n          },\n          \"description\": \"Rate Control Mode.\"\n        }\n      ]\n    },\n    \"RawFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AacRawFormat\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"rawFormat\"\n          },\n          \"description\": \"Enables LATM/LOAS AAC output. Note that if you use LATM/LOAS AAC in an output, you must choose \\\"No container\\\" for the output container.\"\n        }\n      ]\n    },\n    \"SampleRate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin8000Max96000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sampleRate\"\n          },\n          \"description\": \"Specify the Sample rate in Hz. Valid sample rates depend on the Profile and Coding mode that you select. The following list shows valid sample rates for each Profile and Coding mode. * LC Profile, Coding mode 1.0, 2.0, and\
  \ Receiver Mix: 8000, 12000, 16000, 22050, 24000, 32000, 44100, 48000, 88200, 96000. * LC Profile, Coding mode 5.1: 32000, 44100, 48000, 96000. * HEV1 Profile, Coding mode 1.0 and Receiver Mix: 22050, 24000, 32000, 44100, 48000. * HEV1 Profile, Coding mode 2.0 and 5.1: 32000, 44100, 48000, 96000. * HEV2 Profile, Coding mode 2.0: 22050, 24000, 32000, 44100, 48000.\"\n        }\n      ]\n    },\n    \"Specification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AacSpecification\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"specification\"\n          },\n          \"description\": \"Use MPEG-2 AAC instead of MPEG-4 AAC audio for raw or MPEG-2 Transport Stream containers.\"\n        }\n      ]\n    },\n    \"VbrQuality\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AacVbrQuality\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"vbrQuality\"\n          },\n          \"description\"\
  : \"VBR Quality Level - Only used if rate_control_mode is VBR.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-aac-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: AacSettings
---
