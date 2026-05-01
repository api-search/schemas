---
description: Required when you set (Codec) under (VideoDescription)>(CodecSettings) to the value VP9.
layout: schema
name: Vp9Settings
properties_list:
- description: ''
  name: Bitrate
  type: object
- description: ''
  name: FramerateControl
  type: object
- description: ''
  name: FramerateConversionAlgorithm
  type: object
- description: ''
  name: FramerateDenominator
  type: object
- description: ''
  name: FramerateNumerator
  type: object
- description: ''
  name: GopSize
  type: object
- description: ''
  name: HrdBufferSize
  type: object
- description: ''
  name: MaxBitrate
  type: object
- description: ''
  name: ParControl
  type: object
- description: ''
  name: ParDenominator
  type: object
- description: ''
  name: ParNumerator
  type: object
- description: ''
  name: QualityTuningLevel
  type: object
- description: ''
  name: RateControlMode
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-vp9-settings-schema.json
slug: mediaconvert-api-vp9-settings
source_filename: mediaconvert-api-vp9-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-vp9-settings-schema.json\",\n  \"title\": \"Vp9Settings\",\n  \"description\": \"Required when you set (Codec) under (VideoDescription)>(CodecSettings) to the value VP9.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Bitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1000Max480000000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bitrate\"\n          },\n          \"description\": \"Target bitrate in bits/second. For example, enter five megabits per second as 5000000.\"\n        }\n      ]\n    },\n    \"FramerateControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Vp9FramerateControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateControl\"\
  \n          },\n          \"description\": \"If you are using the console, use the Framerate setting to specify the frame rate for this output. If you want to keep the same frame rate as the input video, choose Follow source. If you want to do frame rate conversion, choose a frame rate from the dropdown list or choose Custom. The framerates shown in the dropdown list are decimal approximations of fractions. If you choose Custom, specify your frame rate as a fraction. If you are creating your transcoding job specification as a JSON file without the console, use FramerateControl to specify which value the service uses for the frame rate for this output. Choose INITIALIZE_FROM_SOURCE if you want the service to use the frame rate from the input. Choose SPECIFIED if you want the service to use the frame rate you specify in the settings FramerateNumerator and FramerateDenominator.\"\n        }\n      ]\n    },\n    \"FramerateConversionAlgorithm\": {\n      \"allOf\": [\n        {\n        \
  \  \"$ref\": \"#/components/schemas/Vp9FramerateConversionAlgorithm\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateConversionAlgorithm\"\n          },\n          \"description\": \"Choose the method that you want MediaConvert to use when increasing or decreasing the frame rate. We recommend using drop duplicate (DUPLICATE_DROP) for numerically simple conversions, such as 60 fps to 30 fps. For numerically complex conversions, you can use interpolate (INTERPOLATE) to avoid stutter. This results in a smooth picture, but might introduce undesirable video artifacts. For complex frame rate conversions, especially if your source video has already been converted from its original cadence, use FrameFormer (FRAMEFORMER) to do motion-compensated interpolation. FrameFormer chooses the best conversion method frame by frame. Note that using FrameFormer increases the transcoding time and incurs a significant add-on cost.\"\n        }\n      ]\n    },\n    \"FramerateDenominator\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateDenominator\"\n          },\n          \"description\": \"When you use the API for transcode jobs that use frame rate conversion, specify the frame rate as a fraction. For example, 24000 / 1001 = 23.976 fps. Use FramerateDenominator to specify the denominator of this fraction. In this example, use 1001 for the value of FramerateDenominator. When you use the console for transcode jobs that use frame rate conversion, provide the value as a decimal number for Framerate. In this example, specify 23.976.\"\n        }\n      ]\n    },\n    \"FramerateNumerator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateNumerator\"\n          },\n          \"description\": \"When you\
  \ use the API for transcode jobs that use frame rate conversion, specify the frame rate as a fraction. For example, 24000 / 1001 = 23.976 fps. Use FramerateNumerator to specify the numerator of this fraction. In this example, use 24000 for the value of FramerateNumerator. When you use the console for transcode jobs that use frame rate conversion, provide the value as a decimal number for Framerate. In this example, specify 23.976.\"\n        }\n      ]\n    },\n    \"GopSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gopSize\"\n          },\n          \"description\": \"GOP Length (keyframe interval) in frames. Must be greater than zero.\"\n        }\n      ]\n    },\n    \"HrdBufferSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max47185920\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hrdBufferSize\"\
  \n          },\n          \"description\": \"Size of buffer (HRD buffer model) in bits. For example, enter five megabits as 5000000.\"\n        }\n      ]\n    },\n    \"MaxBitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1000Max480000000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxBitrate\"\n          },\n          \"description\": \"Ignore this setting unless you set qualityTuningLevel to MULTI_PASS. Optional. Specify the maximum bitrate in bits/second. For example, enter five megabits per second as 5000000. The default behavior uses twice the target bitrate as the maximum bitrate.\"\n        }\n      ]\n    },\n    \"ParControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Vp9ParControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"parControl\"\n          },\n          \"description\": \"Optional. Specify how the service determines the pixel aspect\
  \ ratio for this output. The default behavior is to use the same pixel aspect ratio as your input video.\"\n        }\n      ]\n    },\n    \"ParDenominator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"parDenominator\"\n          },\n          \"description\": \"Required when you set Pixel aspect ratio (parControl) to SPECIFIED. On the console, this corresponds to any value other than Follow source. When you specify an output pixel aspect ratio (PAR) that is different from your input video PAR, provide your output PAR as a ratio. For example, for D1/DV NTSC widescreen, you would specify the ratio 40:33. In this example, the value for parDenominator is 33.\"\n        }\n      ]\n    },\n    \"ParNumerator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2147483647\"\n        },\n        {\n          \"xml\":\
  \ {\n            \"name\": \"parNumerator\"\n          },\n          \"description\": \"Required when you set Pixel aspect ratio (parControl) to SPECIFIED. On the console, this corresponds to any value other than Follow source. When you specify an output pixel aspect ratio (PAR) that is different from your input video PAR, provide your output PAR as a ratio. For example, for D1/DV NTSC widescreen, you would specify the ratio 40:33. In this example, the value for parNumerator is 40.\"\n        }\n      ]\n    },\n    \"QualityTuningLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Vp9QualityTuningLevel\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"qualityTuningLevel\"\n          },\n          \"description\": \"Optional. Use Quality tuning level (qualityTuningLevel) to choose how you want to trade off encoding speed for output video quality. The default behavior is faster, lower quality, multi-pass encoding.\"\n        }\n  \
  \    ]\n    },\n    \"RateControlMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Vp9RateControlMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"rateControlMode\"\n          },\n          \"description\": \"With the VP9 codec, you can use only the variable bitrate (VBR) rate control mode.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-vp9-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Vp9Settings
---
