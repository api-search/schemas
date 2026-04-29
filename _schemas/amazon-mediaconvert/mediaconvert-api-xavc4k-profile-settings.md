---
description: Required when you set (Profile) under (VideoDescription)>(CodecSettings)>(XavcSettings) to the value XAVC_4K.
layout: schema
name: Xavc4kProfileSettings
properties_list:
- description: ''
  name: BitrateClass
  type: object
- description: ''
  name: CodecProfile
  type: object
- description: ''
  name: FlickerAdaptiveQuantization
  type: object
- description: ''
  name: GopBReference
  type: object
- description: ''
  name: GopClosedCadence
  type: object
- description: ''
  name: HrdBufferSize
  type: object
- description: ''
  name: QualityTuningLevel
  type: object
- description: ''
  name: Slices
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-xavc4k-profile-settings-schema.json
slug: mediaconvert-api-xavc4k-profile-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-xavc4k-profile-settings-schema.json\",\n  \"title\": \"Xavc4kProfileSettings\",\n  \"description\": \"Required when you set (Profile) under (VideoDescription)>(CodecSettings)>(XavcSettings) to the value XAVC_4K.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BitrateClass\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Xavc4kProfileBitrateClass\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bitrateClass\"\n          },\n          \"description\": \"Specify the XAVC 4k (Long GOP) Bitrate Class to set the bitrate of your output. Outputs of the same class have similar image quality over the operating points that are valid for that class.\"\n        }\n      ]\n    },\n    \"CodecProfile\": {\n      \"allOf\": [\n       \
  \ {\n          \"$ref\": \"#/components/schemas/Xavc4kProfileCodecProfile\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"codecProfile\"\n          },\n          \"description\": \"Specify the codec profile for this output. Choose High, 8-bit, 4:2:0 (HIGH) or High, 10-bit, 4:2:2 (HIGH_422). These profiles are specified in ITU-T H.264.\"\n        }\n      ]\n    },\n    \"FlickerAdaptiveQuantization\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XavcFlickerAdaptiveQuantization\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flickerAdaptiveQuantization\"\n          },\n          \"description\": \"The best way to set up adaptive quantization is to keep the default value, Auto (AUTO), for the setting Adaptive quantization (XavcAdaptiveQuantization). When you do so, MediaConvert automatically applies the best types of quantization for your video content. Include this setting in your JSON job specification only\
  \ when you choose to change the default value for Adaptive quantization. Enable this setting to have the encoder reduce I-frame pop. I-frame pop appears as a visual flicker that can arise when the encoder saves bits by copying some macroblocks many times from frame to frame, and then refreshes them at the I-frame. When you enable this setting, the encoder updates these macroblocks slightly more often to smooth out the flicker. This setting is disabled by default. Related setting: In addition to enabling this setting, you must also set Adaptive quantization (adaptiveQuantization) to a value other than Off (OFF) or Auto (AUTO). Use Adaptive quantization to adjust the degree of smoothing that Flicker adaptive quantization provides.\"\n        }\n      ]\n    },\n    \"GopBReference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XavcGopBReference\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gopBReference\"\n          },\n        \
  \  \"description\": \"Specify whether the encoder uses B-frames as reference frames for other pictures in the same GOP. Choose Allow (ENABLED) to allow the encoder to use B-frames as reference frames. Choose Don't allow (DISABLED) to prevent the encoder from using B-frames as reference frames.\"\n        }\n      ]\n    },\n    \"GopClosedCadence\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gopClosedCadence\"\n          },\n          \"description\": \"Frequency of closed GOPs. In streaming applications, it is recommended that this be set to 1 so a decoder joining mid-stream will receive an IDR frame as quickly as possible. Setting this value to 0 will break output segmenting.\"\n        }\n      ]\n    },\n    \"HrdBufferSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max1152000000\"\n        },\n      \
  \  {\n          \"xml\": {\n            \"name\": \"hrdBufferSize\"\n          },\n          \"description\": \"Specify the size of the buffer that MediaConvert uses in the HRD buffer model for this output. Specify this value in bits; for example, enter five megabits as 5000000. When you don't set this value, or you set it to zero, MediaConvert calculates the default by doubling the bitrate of this output point.\"\n        }\n      ]\n    },\n    \"QualityTuningLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Xavc4kProfileQualityTuningLevel\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"qualityTuningLevel\"\n          },\n          \"description\": \"Optional. Use Quality tuning level (qualityTuningLevel) to choose how you want to trade off encoding speed for output video quality. The default behavior is faster, lower quality, single-pass encoding.\"\n        }\n      ]\n    },\n    \"Slices\": {\n      \"allOf\": [\n      \
  \  {\n          \"$ref\": \"#/components/schemas/__integerMin8Max12\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"slices\"\n          },\n          \"description\": \"Number of slices per picture. Must be less than or equal to the number of macroblock rows for progressive pictures, and less than or equal to half the number of macroblock rows for interlaced pictures.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-xavc4k-profile-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Xavc4kProfileSettings
---
