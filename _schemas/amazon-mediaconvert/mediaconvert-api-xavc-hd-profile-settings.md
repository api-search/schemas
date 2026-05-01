---
description: Required when you set (Profile) under (VideoDescription)>(CodecSettings)>(XavcSettings) to the value XAVC_HD.
layout: schema
name: XavcHdProfileSettings
properties_list:
- description: ''
  name: BitrateClass
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
  name: InterlaceMode
  type: object
- description: ''
  name: QualityTuningLevel
  type: object
- description: ''
  name: Slices
  type: object
- description: ''
  name: Telecine
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-xavc-hd-profile-settings-schema.json
slug: mediaconvert-api-xavc-hd-profile-settings
source_filename: mediaconvert-api-xavc-hd-profile-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-xavc-hd-profile-settings-schema.json\",\n  \"title\": \"XavcHdProfileSettings\",\n  \"description\": \"Required when you set (Profile) under (VideoDescription)>(CodecSettings)>(XavcSettings) to the value XAVC_HD.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BitrateClass\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XavcHdProfileBitrateClass\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bitrateClass\"\n          },\n          \"description\": \"Specify the XAVC HD (Long GOP) Bitrate Class to set the bitrate of your output. Outputs of the same class have similar image quality over the operating points that are valid for that class.\"\n        }\n      ]\n    },\n    \"FlickerAdaptiveQuantization\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/XavcFlickerAdaptiveQuantization\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flickerAdaptiveQuantization\"\n          },\n          \"description\": \"The best way to set up adaptive quantization is to keep the default value, Auto (AUTO), for the setting Adaptive quantization (XavcAdaptiveQuantization). When you do so, MediaConvert automatically applies the best types of quantization for your video content. Include this setting in your JSON job specification only when you choose to change the default value for Adaptive quantization. Enable this setting to have the encoder reduce I-frame pop. I-frame pop appears as a visual flicker that can arise when the encoder saves bits by copying some macroblocks many times from frame to frame, and then refreshes them at the I-frame. When you enable this setting, the encoder updates these macroblocks slightly more often to smooth out the flicker. This setting is disabled\
  \ by default. Related setting: In addition to enabling this setting, you must also set Adaptive quantization (adaptiveQuantization) to a value other than Off (OFF) or Auto (AUTO). Use Adaptive quantization to adjust the degree of smoothing that Flicker adaptive quantization provides.\"\n        }\n      ]\n    },\n    \"GopBReference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XavcGopBReference\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gopBReference\"\n          },\n          \"description\": \"Specify whether the encoder uses B-frames as reference frames for other pictures in the same GOP. Choose Allow (ENABLED) to allow the encoder to use B-frames as reference frames. Choose Don't allow (DISABLED) to prevent the encoder from using B-frames as reference frames.\"\n        }\n      ]\n    },\n    \"GopClosedCadence\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"gopClosedCadence\"\n          },\n          \"description\": \"Frequency of closed GOPs. In streaming applications, it is recommended that this be set to 1 so a decoder joining mid-stream will receive an IDR frame as quickly as possible. Setting this value to 0 will break output segmenting.\"\n        }\n      ]\n    },\n    \"HrdBufferSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max1152000000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hrdBufferSize\"\n          },\n          \"description\": \"Specify the size of the buffer that MediaConvert uses in the HRD buffer model for this output. Specify this value in bits; for example, enter five megabits as 5000000. When you don't set this value, or you set it to zero, MediaConvert calculates the default by doubling the bitrate of this output point.\"\n        }\n      ]\n    },\n    \"InterlaceMode\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XavcInterlaceMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"interlaceMode\"\n          },\n          \"description\": \"Choose the scan line type for the output. Keep the default value, Progressive (PROGRESSIVE) to create a progressive output, regardless of the scan type of your input. Use Top field first (TOP_FIELD) or Bottom field first (BOTTOM_FIELD) to create an output that's interlaced with the same field polarity throughout. Use Follow, default top (FOLLOW_TOP_FIELD) or Follow, default bottom (FOLLOW_BOTTOM_FIELD) to produce outputs with the same field polarity as the source. For jobs that have multiple inputs, the output field polarity might change over the course of the output. Follow behavior depends on the input scan type. If the source is interlaced, the output will be interlaced with the same polarity as the source. If the source is progressive, the output will be interlaced\
  \ with top field bottom field first, depending on which of the Follow options you choose.\"\n        }\n      ]\n    },\n    \"QualityTuningLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XavcHdProfileQualityTuningLevel\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"qualityTuningLevel\"\n          },\n          \"description\": \"Optional. Use Quality tuning level (qualityTuningLevel) to choose how you want to trade off encoding speed for output video quality. The default behavior is faster, lower quality, single-pass encoding.\"\n        }\n      ]\n    },\n    \"Slices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin4Max12\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"slices\"\n          },\n          \"description\": \"Number of slices per picture. Must be less than or equal to the number of macroblock rows for progressive pictures, and less than or equal\
  \ to half the number of macroblock rows for interlaced pictures.\"\n        }\n      ]\n    },\n    \"Telecine\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XavcHdProfileTelecine\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"telecine\"\n          },\n          \"description\": \"Ignore this setting unless you set Frame rate (framerateNumerator divided by framerateDenominator) to 29.970. If your input framerate is 23.976, choose Hard (HARD). Otherwise, keep the default value None (NONE). For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/working-with-telecine-and-inverse-telecine.html.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-xavc-hd-profile-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: XavcHdProfileSettings
---
