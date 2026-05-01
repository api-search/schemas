---
description: Required when you set (Codec) under (VideoDescription)>(CodecSettings) to the value PRORES.
layout: schema
name: ProresSettings
properties_list:
- description: ''
  name: ChromaSampling
  type: object
- description: ''
  name: CodecProfile
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
  name: InterlaceMode
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
  name: ScanTypeConversionMode
  type: object
- description: ''
  name: SlowPal
  type: object
- description: ''
  name: Telecine
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-prores-settings-schema.json
slug: mediaconvert-api-prores-settings
source_filename: mediaconvert-api-prores-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-prores-settings-schema.json\",\n  \"title\": \"ProresSettings\",\n  \"description\": \"Required when you set (Codec) under (VideoDescription)>(CodecSettings) to the value PRORES.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChromaSampling\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProresChromaSampling\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"chromaSampling\"\n          },\n          \"description\": \"This setting applies only to ProRes 4444 and ProRes 4444 XQ outputs that you create from inputs that use 4:4:4 chroma sampling. Set Preserve 4:4:4 sampling (PRESERVE_444_SAMPLING) to allow outputs to also use 4:4:4 chroma sampling. You must specify a value for this setting when your output codec profile supports\
  \ 4:4:4 chroma sampling. Related Settings: When you set Chroma sampling to Preserve 4:4:4 sampling (PRESERVE_444_SAMPLING), you must choose an output codec profile that supports 4:4:4 chroma sampling. These values for Profile (CodecProfile) support 4:4:4 chroma sampling: Apple ProRes 4444 (APPLE_PRORES_4444) or Apple ProRes 4444 XQ (APPLE_PRORES_4444_XQ). When you set Chroma sampling to Preserve 4:4:4 sampling, you must disable all video preprocessors except for Nexguard file marker (PartnerWatermarking). When you set Chroma sampling to Preserve 4:4:4 sampling and use framerate conversion, you must set Frame rate conversion algorithm (FramerateConversionAlgorithm) to Drop duplicate (DUPLICATE_DROP).\"\n        }\n      ]\n    },\n    \"CodecProfile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProresCodecProfile\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"codecProfile\"\n          },\n          \"description\": \"Use Profile\
  \ (ProResCodecProfile) to specify the type of Apple ProRes codec to use for this output.\"\n        }\n      ]\n    },\n    \"FramerateControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProresFramerateControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateControl\"\n          },\n          \"description\": \"If you are using the console, use the Framerate setting to specify the frame rate for this output. If you want to keep the same frame rate as the input video, choose Follow source. If you want to do frame rate conversion, choose a frame rate from the dropdown list or choose Custom. The framerates shown in the dropdown list are decimal approximations of fractions. If you choose Custom, specify your frame rate as a fraction. If you are creating your transcoding job specification as a JSON file without the console, use FramerateControl to specify which value the service uses for the frame rate for this output. Choose\
  \ INITIALIZE_FROM_SOURCE if you want the service to use the frame rate from the input. Choose SPECIFIED if you want the service to use the frame rate you specify in the settings FramerateNumerator and FramerateDenominator.\"\n        }\n      ]\n    },\n    \"FramerateConversionAlgorithm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProresFramerateConversionAlgorithm\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateConversionAlgorithm\"\n          },\n          \"description\": \"Choose the method that you want MediaConvert to use when increasing or decreasing the frame rate. We recommend using drop duplicate (DUPLICATE_DROP) for numerically simple conversions, such as 60 fps to 30 fps. For numerically complex conversions, you can use interpolate (INTERPOLATE) to avoid stutter. This results in a smooth picture, but might introduce undesirable video artifacts. For complex frame rate conversions, especially if your source\
  \ video has already been converted from its original cadence, use FrameFormer (FRAMEFORMER) to do motion-compensated interpolation. FrameFormer chooses the best conversion method frame by frame. Note that using FrameFormer increases the transcoding time and incurs a significant add-on cost.\"\n        }\n      ]\n    },\n    \"FramerateDenominator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateDenominator\"\n          },\n          \"description\": \"When you use the API for transcode jobs that use frame rate conversion, specify the frame rate as a fraction. For example, 24000 / 1001 = 23.976 fps. Use FramerateDenominator to specify the denominator of this fraction. In this example, use 1001 for the value of FramerateDenominator. When you use the console for transcode jobs that use frame rate conversion, provide the value as a decimal number for Framerate.\
  \ In this example, specify 23.976.\"\n        }\n      ]\n    },\n    \"FramerateNumerator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateNumerator\"\n          },\n          \"description\": \"When you use the API for transcode jobs that use frame rate conversion, specify the frame rate as a fraction. For example, 24000 / 1001 = 23.976 fps. Use FramerateNumerator to specify the numerator of this fraction. In this example, use 24000 for the value of FramerateNumerator. When you use the console for transcode jobs that use frame rate conversion, provide the value as a decimal number for Framerate. In this example, specify 23.976.\"\n        }\n      ]\n    },\n    \"InterlaceMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProresInterlaceMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"\
  interlaceMode\"\n          },\n          \"description\": \"Choose the scan line type for the output. Keep the default value, Progressive (PROGRESSIVE) to create a progressive output, regardless of the scan type of your input. Use Top field first (TOP_FIELD) or Bottom field first (BOTTOM_FIELD) to create an output that's interlaced with the same field polarity throughout. Use Follow, default top (FOLLOW_TOP_FIELD) or Follow, default bottom (FOLLOW_BOTTOM_FIELD) to produce outputs with the same field polarity as the source. For jobs that have multiple inputs, the output field polarity might change over the course of the output. Follow behavior depends on the input scan type. If the source is interlaced, the output will be interlaced with the same polarity as the source. If the source is progressive, the output will be interlaced with top field bottom field first, depending on which of the Follow options you choose.\"\n        }\n      ]\n    },\n    \"ParControl\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/ProresParControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"parControl\"\n          },\n          \"description\": \"Optional. Specify how the service determines the pixel aspect ratio (PAR) for this output. The default behavior, Follow source (INITIALIZE_FROM_SOURCE), uses the PAR from your input video for your output. To specify a different PAR in the console, choose any value other than Follow source. To specify a different PAR by editing the JSON job specification, choose SPECIFIED. When you choose SPECIFIED for this setting, you must also specify values for the parNumerator and parDenominator settings.\"\n        }\n      ]\n    },\n    \"ParDenominator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"parDenominator\"\n          },\n          \"description\": \"Required\
  \ when you set Pixel aspect ratio (parControl) to SPECIFIED. On the console, this corresponds to any value other than Follow source. When you specify an output pixel aspect ratio (PAR) that is different from your input video PAR, provide your output PAR as a ratio. For example, for D1/DV NTSC widescreen, you would specify the ratio 40:33. In this example, the value for parDenominator is 33.\"\n        }\n      ]\n    },\n    \"ParNumerator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"parNumerator\"\n          },\n          \"description\": \"Required when you set Pixel aspect ratio (parControl) to SPECIFIED. On the console, this corresponds to any value other than Follow source. When you specify an output pixel aspect ratio (PAR) that is different from your input video PAR, provide your output PAR as a ratio. For example, for D1/DV NTSC widescreen, you would\
  \ specify the ratio 40:33. In this example, the value for parNumerator is 40.\"\n        }\n      ]\n    },\n    \"ScanTypeConversionMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProresScanTypeConversionMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scanTypeConversionMode\"\n          },\n          \"description\": \"Use this setting for interlaced outputs, when your output frame rate is half of your input frame rate. In this situation, choose Optimized interlacing (INTERLACED_OPTIMIZE) to create a better quality interlaced output. In this case, each progressive frame from the input corresponds to an interlaced field in the output. Keep the default value, Basic interlacing (INTERLACED), for all other output frame rates. With basic interlacing, MediaConvert performs any frame rate conversion first and then interlaces the frames. When you choose Optimized interlacing and you set your output frame rate to a value that isn't\
  \ suitable for optimized interlacing, MediaConvert automatically falls back to basic interlacing. Required settings: To use optimized interlacing, you must set Telecine (telecine) to None (NONE) or Soft (SOFT). You can't use optimized interlacing for hard telecine outputs. You must also set Interlace mode (interlaceMode) to a value other than Progressive (PROGRESSIVE).\"\n        }\n      ]\n    },\n    \"SlowPal\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProresSlowPal\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"slowPal\"\n          },\n          \"description\": \"Ignore this setting unless your input frame rate is 23.976 or 24 frames per second (fps). Enable slow PAL to create a 25 fps output. When you enable slow PAL, MediaConvert relabels the video frames to 25 fps and resamples your audio to keep it synchronized with the video. Note that enabling this setting will slightly reduce the duration of your video. Required\
  \ settings: You must also set Framerate to 25. In your JSON job specification, set (framerateControl) to (SPECIFIED), (framerateNumerator) to 25 and (framerateDenominator) to 1.\"\n        }\n      ]\n    },\n    \"Telecine\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProresTelecine\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"telecine\"\n          },\n          \"description\": \"When you do frame rate conversion from 23.976 frames per second (fps) to 29.97 fps, and your output scan type is interlaced, you can optionally enable hard telecine (HARD) to create a smoother picture. When you keep the default value, None (NONE), MediaConvert does a standard frame rate conversion to 29.97 without doing anything with the field polarity to create a smoother picture.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-prores-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ProresSettings
---
