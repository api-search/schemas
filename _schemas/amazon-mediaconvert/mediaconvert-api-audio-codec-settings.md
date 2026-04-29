---
description: Settings related to audio encoding. The settings in this group vary depending on the value that you choose for your audio codec.
layout: schema
name: AudioCodecSettings
properties_list:
- description: ''
  name: AacSettings
  type: object
- description: ''
  name: Ac3Settings
  type: object
- description: ''
  name: AiffSettings
  type: object
- description: ''
  name: Codec
  type: object
- description: ''
  name: Eac3AtmosSettings
  type: object
- description: ''
  name: Eac3Settings
  type: object
- description: ''
  name: Mp2Settings
  type: object
- description: ''
  name: Mp3Settings
  type: object
- description: ''
  name: OpusSettings
  type: object
- description: ''
  name: VorbisSettings
  type: object
- description: ''
  name: WavSettings
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-audio-codec-settings-schema.json
slug: mediaconvert-api-audio-codec-settings
source_filename: mediaconvert-api-audio-codec-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-audio-codec-settings-schema.json\",\n  \"title\": \"AudioCodecSettings\",\n  \"description\": \"Settings related to audio encoding. The settings in this group vary depending on the value that you choose for your audio codec.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AacSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AacSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"aacSettings\"\n          },\n          \"description\": \"Required when you set (Codec) under (AudioDescriptions)>(CodecSettings) to the value AAC. The service accepts one of two mutually exclusive groups of AAC settings--VBR and CBR. To select one of these modes, set the value of Bitrate control mode (rateControlMode) to \\\"VBR\\\"\
  \ or \\\"CBR\\\". In VBR mode, you control the audio quality with the setting VBR quality (vbrQuality). In CBR mode, you use the setting Bitrate (bitrate). Defaults and valid values depend on the rate control mode.\"\n        }\n      ]\n    },\n    \"Ac3Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ac3Settings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ac3Settings\"\n          },\n          \"description\": \"Required when you set (Codec) under (AudioDescriptions)>(CodecSettings) to the value AC3.\"\n        }\n      ]\n    },\n    \"AiffSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AiffSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"aiffSettings\"\n          },\n          \"description\": \"Required when you set (Codec) under (AudioDescriptions)>(CodecSettings) to the value AIFF.\"\n        }\n      ]\n    },\n    \"Codec\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/AudioCodec\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"codec\"\n          },\n          \"description\": \"Choose the audio codec for this output. Note that the option Dolby Digital passthrough (PASSTHROUGH) applies only to Dolby Digital and Dolby Digital Plus audio inputs. Make sure that you choose a codec that's supported with your output container: https://docs.aws.amazon.com/mediaconvert/latest/ug/reference-codecs-containers.html#reference-codecs-containers-output-audio For audio-only outputs, make sure that both your input audio codec and your output audio codec are supported for audio-only workflows. For more information, see: https://docs.aws.amazon.com/mediaconvert/latest/ug/reference-codecs-containers-input.html#reference-codecs-containers-input-audio-only and https://docs.aws.amazon.com/mediaconvert/latest/ug/reference-codecs-containers.html#audio-only-output\"\n        }\n      ]\n    },\n\
  \    \"Eac3AtmosSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3AtmosSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"eac3AtmosSettings\"\n          },\n          \"description\": \"Required when you set (Codec) under (AudioDescriptions)>(CodecSettings) to the value EAC3_ATMOS.\"\n        }\n      ]\n    },\n    \"Eac3Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3Settings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"eac3Settings\"\n          },\n          \"description\": \"Required when you set (Codec) under (AudioDescriptions)>(CodecSettings) to the value EAC3.\"\n        }\n      ]\n    },\n    \"Mp2Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mp2Settings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mp2Settings\"\n          },\n          \"description\": \"Required\
  \ when you set (Codec) under (AudioDescriptions)>(CodecSettings) to the value MP2.\"\n        }\n      ]\n    },\n    \"Mp3Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mp3Settings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mp3Settings\"\n          },\n          \"description\": \"Required when you set Codec, under AudioDescriptions>CodecSettings, to the value MP3.\"\n        }\n      ]\n    },\n    \"OpusSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OpusSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"opusSettings\"\n          },\n          \"description\": \"Required when you set Codec, under AudioDescriptions>CodecSettings, to the value OPUS.\"\n        }\n      ]\n    },\n    \"VorbisSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VorbisSettings\"\n        },\n        {\n          \"xml\": {\n   \
  \         \"name\": \"vorbisSettings\"\n          },\n          \"description\": \"Required when you set Codec, under AudioDescriptions>CodecSettings, to the value Vorbis.\"\n        }\n      ]\n    },\n    \"WavSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WavSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"wavSettings\"\n          },\n          \"description\": \"Required when you set (Codec) under (AudioDescriptions)>(CodecSettings) to the value WAV.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-audio-codec-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AudioCodecSettings
---
