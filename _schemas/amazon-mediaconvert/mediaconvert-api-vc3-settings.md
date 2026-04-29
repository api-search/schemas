---
description: Required when you set (Codec) under (VideoDescription)>(CodecSettings) to the value VC3
layout: schema
name: Vc3Settings
properties_list:
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
  name: InterlaceMode
  type: object
- description: ''
  name: ScanTypeConversionMode
  type: object
- description: ''
  name: SlowPal
  type: object
- description: ''
  name: Telecine
  type: object
- description: ''
  name: Vc3Class
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-vc3-settings-schema.json
slug: mediaconvert-api-vc3-settings
source_filename: mediaconvert-api-vc3-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-vc3-settings-schema.json\",\n  \"title\": \"Vc3Settings\",\n  \"description\": \"Required when you set (Codec) under (VideoDescription)>(CodecSettings) to the value VC3\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FramerateControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Vc3FramerateControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateControl\"\n          },\n          \"description\": \"If you are using the console, use the Framerate setting to specify the frame rate for this output. If you want to keep the same frame rate as the input video, choose Follow source. If you want to do frame rate conversion, choose a frame rate from the dropdown list or choose Custom. The framerates shown in the dropdown\
  \ list are decimal approximations of fractions. If you choose Custom, specify your frame rate as a fraction. If you are creating your transcoding job specification as a JSON file without the console, use FramerateControl to specify which value the service uses for the frame rate for this output. Choose INITIALIZE_FROM_SOURCE if you want the service to use the frame rate from the input. Choose SPECIFIED if you want the service to use the frame rate you specify in the settings FramerateNumerator and FramerateDenominator.\"\n        }\n      ]\n    },\n    \"FramerateConversionAlgorithm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Vc3FramerateConversionAlgorithm\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateConversionAlgorithm\"\n          },\n          \"description\": \"Choose the method that you want MediaConvert to use when increasing or decreasing the frame rate. We recommend using drop duplicate (DUPLICATE_DROP) for\
  \ numerically simple conversions, such as 60 fps to 30 fps. For numerically complex conversions, you can use interpolate (INTERPOLATE) to avoid stutter. This results in a smooth picture, but might introduce undesirable video artifacts. For complex frame rate conversions, especially if your source video has already been converted from its original cadence, use FrameFormer (FRAMEFORMER) to do motion-compensated interpolation. FrameFormer chooses the best conversion method frame by frame. Note that using FrameFormer increases the transcoding time and incurs a significant add-on cost.\"\n        }\n      ]\n    },\n    \"FramerateDenominator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max1001\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateDenominator\"\n          },\n          \"description\": \"When you use the API for transcode jobs that use frame rate conversion, specify the frame rate as a fraction. For\
  \ example, 24000 / 1001 = 23.976 fps. Use FramerateDenominator to specify the denominator of this fraction. In this example, use 1001 for the value of FramerateDenominator. When you use the console for transcode jobs that use frame rate conversion, provide the value as a decimal number for Framerate. In this example, specify 23.976.\"\n        }\n      ]\n    },\n    \"FramerateNumerator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin24Max60000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateNumerator\"\n          },\n          \"description\": \"When you use the API for transcode jobs that use frame rate conversion, specify the frame rate as a fraction. For example, 24000 / 1001 = 23.976 fps. Use FramerateNumerator to specify the numerator of this fraction. In this example, use 24000 for the value of FramerateNumerator. When you use the console for transcode jobs that use frame rate conversion, provide the value\
  \ as a decimal number for Framerate. In this example, specify 23.976.\"\n        }\n      ]\n    },\n    \"InterlaceMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Vc3InterlaceMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"interlaceMode\"\n          },\n          \"description\": \"Optional. Choose the scan line type for this output. If you don't specify a value, MediaConvert will create a progressive output.\"\n        }\n      ]\n    },\n    \"ScanTypeConversionMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Vc3ScanTypeConversionMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scanTypeConversionMode\"\n          },\n          \"description\": \"Use this setting for interlaced outputs, when your output frame rate is half of your input frame rate. In this situation, choose Optimized interlacing (INTERLACED_OPTIMIZE) to create a better quality interlaced output.\
  \ In this case, each progressive frame from the input corresponds to an interlaced field in the output. Keep the default value, Basic interlacing (INTERLACED), for all other output frame rates. With basic interlacing, MediaConvert performs any frame rate conversion first and then interlaces the frames. When you choose Optimized interlacing and you set your output frame rate to a value that isn't suitable for optimized interlacing, MediaConvert automatically falls back to basic interlacing. Required settings: To use optimized interlacing, you must set Telecine (telecine) to None (NONE) or Soft (SOFT). You can't use optimized interlacing for hard telecine outputs. You must also set Interlace mode (interlaceMode) to a value other than Progressive (PROGRESSIVE).\"\n        }\n      ]\n    },\n    \"SlowPal\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Vc3SlowPal\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"slowPal\"\n          },\n\
  \          \"description\": \"Ignore this setting unless your input frame rate is 23.976 or 24 frames per second (fps). Enable slow PAL to create a 25 fps output by relabeling the video frames and resampling your audio. Note that enabling this setting will slightly reduce the duration of your video. Related settings: You must also set Framerate to 25. In your JSON job specification, set (framerateControl) to (SPECIFIED), (framerateNumerator) to 25 and (framerateDenominator) to 1.\"\n        }\n      ]\n    },\n    \"Telecine\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Vc3Telecine\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"telecine\"\n          },\n          \"description\": \"When you do frame rate conversion from 23.976 frames per second (fps) to 29.97 fps, and your output scan type is interlaced, you can optionally enable hard telecine (HARD) to create a smoother picture. When you keep the default value, None (NONE), MediaConvert\
  \ does a standard frame rate conversion to 29.97 without doing anything with the field polarity to create a smoother picture.\"\n        }\n      ]\n    },\n    \"Vc3Class\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Vc3Class\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"vc3Class\"\n          },\n          \"description\": \"Specify the VC3 class to choose the quality characteristics for this output. VC3 class, together with the settings Framerate (framerateNumerator and framerateDenominator) and Resolution (height and width), determine your output bitrate. For example, say that your video resolution is 1920x1080 and your framerate is 29.97. Then Class 145 (CLASS_145) gives you an output with a bitrate of approximately 145 Mbps and Class 220 (CLASS_220) gives you and output with a bitrate of approximately 220 Mbps. VC3 class also specifies the color bit depth of your output.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-vc3-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Vc3Settings
---
