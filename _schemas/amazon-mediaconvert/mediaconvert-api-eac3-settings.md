---
description: Required when you set (Codec) under (AudioDescriptions)>(CodecSettings) to the value EAC3.
layout: schema
name: Eac3Settings
properties_list:
- description: ''
  name: AttenuationControl
  type: object
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
  name: DcFilter
  type: object
- description: ''
  name: Dialnorm
  type: object
- description: ''
  name: DynamicRangeCompressionLine
  type: object
- description: ''
  name: DynamicRangeCompressionRf
  type: object
- description: ''
  name: LfeControl
  type: object
- description: ''
  name: LfeFilter
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
  name: MetadataControl
  type: object
- description: ''
  name: PassthroughControl
  type: object
- description: ''
  name: PhaseControl
  type: object
- description: ''
  name: SampleRate
  type: object
- description: ''
  name: StereoDownmix
  type: object
- description: ''
  name: SurroundExMode
  type: object
- description: ''
  name: SurroundMode
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-eac3-settings-schema.json
slug: mediaconvert-api-eac3-settings
source_filename: mediaconvert-api-eac3-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-eac3-settings-schema.json\",\n  \"title\": \"Eac3Settings\",\n  \"description\": \"Required when you set (Codec) under (AudioDescriptions)>(CodecSettings) to the value EAC3.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AttenuationControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3AttenuationControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"attenuationControl\"\n          },\n          \"description\": \"If set to ATTENUATE_3_DB, applies a 3 dB attenuation to the surround channels. Only used for 3/2 coding mode.\"\n        }\n      ]\n    },\n    \"Bitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin32000Max3024000\"\n        },\n        {\n          \"xml\"\
  : {\n            \"name\": \"bitrate\"\n          },\n          \"description\": \"Specify the average bitrate in bits per second. The bitrate that you specify must be a multiple of 8000 within the allowed minimum and maximum values. Leave blank to use the default bitrate for the coding mode you select according ETSI TS 102 366. Valid bitrates for coding mode 1/0: Default: 96000. Minimum: 32000. Maximum: 3024000. Valid bitrates for coding mode 2/0: Default: 192000. Minimum: 96000. Maximum: 3024000. Valid bitrates for coding mode 3/2: Default: 384000. Minimum: 192000. Maximum: 3024000.\"\n        }\n      ]\n    },\n    \"BitstreamMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3BitstreamMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bitstreamMode\"\n          },\n          \"description\": \"Specify the bitstream mode for the E-AC-3 stream that the encoder emits. For more information about the EAC3 bitstream mode, see\
  \ ATSC A/52-2012 (Annex E).\"\n        }\n      ]\n    },\n    \"CodingMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3CodingMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"codingMode\"\n          },\n          \"description\": \"Dolby Digital Plus coding mode. Determines number of channels.\"\n        }\n      ]\n    },\n    \"DcFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3DcFilter\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dcFilter\"\n          },\n          \"description\": \"Activates a DC highpass filter for all input channels.\"\n        }\n      ]\n    },\n    \"Dialnorm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max31\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dialnorm\"\n          },\n          \"description\": \"Sets the dialnorm for the output. If blank and\
  \ input audio is Dolby Digital Plus, dialnorm will be passed through.\"\n        }\n      ]\n    },\n    \"DynamicRangeCompressionLine\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3DynamicRangeCompressionLine\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dynamicRangeCompressionLine\"\n          },\n          \"description\": \"Choose the Dolby Digital dynamic range control (DRC) profile that MediaConvert uses when encoding the metadata in the Dolby Digital stream for the line operating mode. Related setting: When you use this setting, MediaConvert ignores any value you provide for Dynamic range compression profile (DynamicRangeCompressionProfile). For information about the Dolby Digital DRC operating modes and profiles, see the Dynamic Range Control chapter of the Dolby Metadata Guide at https://developer.dolby.com/globalassets/professional/documents/dolby-metadata-guide.pdf.\"\n        }\n      ]\n    },\n    \"DynamicRangeCompressionRf\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3DynamicRangeCompressionRf\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dynamicRangeCompressionRf\"\n          },\n          \"description\": \"Choose the Dolby Digital dynamic range control (DRC) profile that MediaConvert uses when encoding the metadata in the Dolby Digital stream for the RF operating mode. Related setting: When you use this setting, MediaConvert ignores any value you provide for Dynamic range compression profile (DynamicRangeCompressionProfile). For information about the Dolby Digital DRC operating modes and profiles, see the Dynamic Range Control chapter of the Dolby Metadata Guide at https://developer.dolby.com/globalassets/professional/documents/dolby-metadata-guide.pdf.\"\n        }\n      ]\n    },\n    \"LfeControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3LfeControl\"\n        },\n        {\n          \"xml\": {\n\
  \            \"name\": \"lfeControl\"\n          },\n          \"description\": \"When encoding 3/2 audio, controls whether the LFE channel is enabled\"\n        }\n      ]\n    },\n    \"LfeFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3LfeFilter\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"lfeFilter\"\n          },\n          \"description\": \"Applies a 120Hz lowpass filter to the LFE channel prior to encoding. Only valid with 3_2_LFE coding mode.\"\n        }\n      ]\n    },\n    \"LoRoCenterMixLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMinNegative60Max3\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"loRoCenterMixLevel\"\n          },\n          \"description\": \"Specify a value for the following Dolby Digital Plus setting: Left only/Right only center mix (Lo/Ro center). MediaConvert uses this value for downmixing. How the service uses\
  \ this value depends on the value that you choose for Stereo downmix (Eac3StereoDownmix). Valid values: 3.0, 1.5, 0.0, -1.5, -3.0, -4.5, -6.0, and -60. The value -60 mutes the channel. This setting applies only if you keep the default value of 3/2 - L, R, C, Ls, Rs (CODING_MODE_3_2) for the setting Coding mode (Eac3CodingMode). If you choose a different value for Coding mode, the service ignores Left only/Right only center (loRoCenterMixLevel).\"\n        }\n      ]\n    },\n    \"LoRoSurroundMixLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMinNegative60MaxNegative1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"loRoSurroundMixLevel\"\n          },\n          \"description\": \"Specify a value for the following Dolby Digital Plus setting: Left only/Right only (Lo/Ro surround). MediaConvert uses this value for downmixing. How the service uses this value depends on the value that you choose for Stereo downmix (Eac3StereoDownmix).\
  \ Valid values: -1.5, -3.0, -4.5, -6.0, and -60. The value -60 mutes the channel. This setting applies only if you keep the default value of 3/2 - L, R, C, Ls, Rs (CODING_MODE_3_2) for the setting Coding mode (Eac3CodingMode). If you choose a different value for Coding mode, the service ignores Left only/Right only surround (loRoSurroundMixLevel).\"\n        }\n      ]\n    },\n    \"LtRtCenterMixLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMinNegative60Max3\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ltRtCenterMixLevel\"\n          },\n          \"description\": \"Specify a value for the following Dolby Digital Plus setting: Left total/Right total center mix (Lt/Rt center). MediaConvert uses this value for downmixing. How the service uses this value depends on the value that you choose for Stereo downmix (Eac3StereoDownmix). Valid values: 3.0, 1.5, 0.0, -1.5, -3.0, -4.5, -6.0, and -60. The value -60 mutes the\
  \ channel. This setting applies only if you keep the default value of 3/2 - L, R, C, Ls, Rs (CODING_MODE_3_2) for the setting Coding mode (Eac3CodingMode). If you choose a different value for Coding mode, the service ignores Left total/Right total center (ltRtCenterMixLevel).\"\n        }\n      ]\n    },\n    \"LtRtSurroundMixLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMinNegative60MaxNegative1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ltRtSurroundMixLevel\"\n          },\n          \"description\": \"Specify a value for the following Dolby Digital Plus setting: Left total/Right total surround mix (Lt/Rt surround). MediaConvert uses this value for downmixing. How the service uses this value depends on the value that you choose for Stereo downmix (Eac3StereoDownmix). Valid values: -1.5, -3.0, -4.5, -6.0, and -60. The value -60 mutes the channel. This setting applies only if you keep the default value of 3/2\
  \ - L, R, C, Ls, Rs (CODING_MODE_3_2) for the setting Coding mode (Eac3CodingMode). If you choose a different value for Coding mode, the service ignores Left total/Right total surround (ltRtSurroundMixLevel).\"\n        }\n      ]\n    },\n    \"MetadataControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3MetadataControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"metadataControl\"\n          },\n          \"description\": \"When set to FOLLOW_INPUT, encoder metadata will be sourced from the DD, DD+, or DolbyE decoder that supplied this audio data. If audio was not supplied from one of these streams, then the static metadata settings will be used.\"\n        }\n      ]\n    },\n    \"PassthroughControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3PassthroughControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"passthroughControl\"\n          },\n         \
  \ \"description\": \"When set to WHEN_POSSIBLE, input DD+ audio will be passed through if it is present on the input. this detection is dynamic over the life of the transcode. Inputs that alternate between DD+ and non-DD+ content will have a consistent DD+ output as the system alternates between passthrough and encoding.\"\n        }\n      ]\n    },\n    \"PhaseControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3PhaseControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"phaseControl\"\n          },\n          \"description\": \"Controls the amount of phase-shift applied to the surround channels. Only used for 3/2 coding mode.\"\n        }\n      ]\n    },\n    \"SampleRate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin48000Max48000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sampleRate\"\n          },\n          \"description\": \"This value is always\
  \ 48000. It represents the sample rate in Hz.\"\n        }\n      ]\n    },\n    \"StereoDownmix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3StereoDownmix\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"stereoDownmix\"\n          },\n          \"description\": \"Choose how the service does stereo downmixing. This setting only applies if you keep the default value of 3/2 - L, R, C, Ls, Rs (CODING_MODE_3_2) for the setting Coding mode (Eac3CodingMode). If you choose a different value for Coding mode, the service ignores Stereo downmix (Eac3StereoDownmix).\"\n        }\n      ]\n    },\n    \"SurroundExMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3SurroundExMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"surroundExMode\"\n          },\n          \"description\": \"When encoding 3/2 audio, sets whether an extra center back surround channel is matrix encoded\
  \ into the left and right surround channels.\"\n        }\n      ]\n    },\n    \"SurroundMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3SurroundMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"surroundMode\"\n          },\n          \"description\": \"When encoding 2/0 audio, sets whether Dolby Surround is matrix encoded into the two channels.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-eac3-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Eac3Settings
---
