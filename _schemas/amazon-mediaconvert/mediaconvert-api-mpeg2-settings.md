---
description: Required when you set (Codec) under (VideoDescription)>(CodecSettings) to the value MPEG2.
layout: schema
name: Mpeg2Settings
properties_list:
- description: ''
  name: AdaptiveQuantization
  type: object
- description: ''
  name: Bitrate
  type: object
- description: ''
  name: CodecLevel
  type: object
- description: ''
  name: CodecProfile
  type: object
- description: ''
  name: DynamicSubGop
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
  name: GopClosedCadence
  type: object
- description: ''
  name: GopSize
  type: object
- description: ''
  name: GopSizeUnits
  type: object
- description: ''
  name: HrdBufferFinalFillPercentage
  type: object
- description: ''
  name: HrdBufferInitialFillPercentage
  type: object
- description: ''
  name: HrdBufferSize
  type: object
- description: ''
  name: InterlaceMode
  type: object
- description: ''
  name: IntraDcPrecision
  type: object
- description: ''
  name: MaxBitrate
  type: object
- description: ''
  name: MinIInterval
  type: object
- description: ''
  name: NumberBFramesBetweenReferenceFrames
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
- description: ''
  name: ScanTypeConversionMode
  type: object
- description: ''
  name: SceneChangeDetect
  type: object
- description: ''
  name: SlowPal
  type: object
- description: ''
  name: Softness
  type: object
- description: ''
  name: SpatialAdaptiveQuantization
  type: object
- description: ''
  name: Syntax
  type: object
- description: ''
  name: Telecine
  type: object
- description: ''
  name: TemporalAdaptiveQuantization
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-mpeg2-settings-schema.json
slug: mediaconvert-api-mpeg2-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mpeg2-settings-schema.json\",\n  \"title\": \"Mpeg2Settings\",\n  \"description\": \"Required when you set (Codec) under (VideoDescription)>(CodecSettings) to the value MPEG2.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdaptiveQuantization\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2AdaptiveQuantization\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"adaptiveQuantization\"\n          },\n          \"description\": \"Specify the strength of any adaptive quantization filters that you enable. The value that you choose here applies to the following settings: Spatial adaptive quantization (spatialAdaptiveQuantization), and Temporal adaptive quantization (temporalAdaptiveQuantization).\"\n        }\n      ]\n \
  \   },\n    \"Bitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1000Max288000000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bitrate\"\n          },\n          \"description\": \"Specify the average bitrate in bits per second. Required for VBR and CBR. For MS Smooth outputs, bitrates must be unique when rounded down to the nearest multiple of 1000.\"\n        }\n      ]\n    },\n    \"CodecLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2CodecLevel\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"codecLevel\"\n          },\n          \"description\": \"Use Level (Mpeg2CodecLevel) to set the MPEG-2 level for the video output.\"\n        }\n      ]\n    },\n    \"CodecProfile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2CodecProfile\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"codecProfile\"\
  \n          },\n          \"description\": \"Use Profile (Mpeg2CodecProfile) to set the MPEG-2 profile for the video output.\"\n        }\n      ]\n    },\n    \"DynamicSubGop\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2DynamicSubGop\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dynamicSubGop\"\n          },\n          \"description\": \"Choose Adaptive to improve subjective video quality for high-motion content. This will cause the service to use fewer B-frames (which infer information based on other frames) for high-motion portions of the video and more B-frames for low-motion portions. The maximum number of B-frames is limited by the value you provide for the setting B frames between reference frames (numberBFramesBetweenReferenceFrames).\"\n        }\n      ]\n    },\n    \"FramerateControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2FramerateControl\"\n        },\n        {\n\
  \          \"xml\": {\n            \"name\": \"framerateControl\"\n          },\n          \"description\": \"If you are using the console, use the Framerate setting to specify the frame rate for this output. If you want to keep the same frame rate as the input video, choose Follow source. If you want to do frame rate conversion, choose a frame rate from the dropdown list or choose Custom. The framerates shown in the dropdown list are decimal approximations of fractions. If you choose Custom, specify your frame rate as a fraction. If you are creating your transcoding job specification as a JSON file without the console, use FramerateControl to specify which value the service uses for the frame rate for this output. Choose INITIALIZE_FROM_SOURCE if you want the service to use the frame rate from the input. Choose SPECIFIED if you want the service to use the frame rate you specify in the settings FramerateNumerator and FramerateDenominator.\"\n        }\n      ]\n    },\n    \"FramerateConversionAlgorithm\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2FramerateConversionAlgorithm\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateConversionAlgorithm\"\n          },\n          \"description\": \"Choose the method that you want MediaConvert to use when increasing or decreasing the frame rate. We recommend using drop duplicate (DUPLICATE_DROP) for numerically simple conversions, such as 60 fps to 30 fps. For numerically complex conversions, you can use interpolate (INTERPOLATE) to avoid stutter. This results in a smooth picture, but might introduce undesirable video artifacts. For complex frame rate conversions, especially if your source video has already been converted from its original cadence, use FrameFormer (FRAMEFORMER) to do motion-compensated interpolation. FrameFormer chooses the best conversion method frame by frame. Note that using FrameFormer increases the transcoding time and incurs a significant add-on cost.\"\
  \n        }\n      ]\n    },\n    \"FramerateDenominator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max1001\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateDenominator\"\n          },\n          \"description\": \"When you use the API for transcode jobs that use frame rate conversion, specify the frame rate as a fraction. For example, 24000 / 1001 = 23.976 fps. Use FramerateDenominator to specify the denominator of this fraction. In this example, use 1001 for the value of FramerateDenominator. When you use the console for transcode jobs that use frame rate conversion, provide the value as a decimal number for Framerate. In this example, specify 23.976.\"\n        }\n      ]\n    },\n    \"FramerateNumerator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin24Max60000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateNumerator\"\n  \
  \        },\n          \"description\": \"When you use the API for transcode jobs that use frame rate conversion, specify the frame rate as a fraction. For example, 24000 / 1001 = 23.976 fps. Use FramerateNumerator to specify the numerator of this fraction. In this example, use 24000 for the value of FramerateNumerator. When you use the console for transcode jobs that use frame rate conversion, provide the value as a decimal number for Framerate. In this example, specify 23.976.\"\n        }\n      ]\n    },\n    \"GopClosedCadence\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gopClosedCadence\"\n          },\n          \"description\": \"Specify the relative frequency of open to closed GOPs in this output. For example, if you want to allow four open GOPs and then require a closed GOP, set this value to 5. When you create a streaming output, we recommend\
  \ that you keep the default value, 1, so that players starting mid-stream receive an IDR frame as quickly as possible. Don't set this value to 0; that would break output segmenting.\"\n        }\n      ]\n    },\n    \"GopSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gopSize\"\n          },\n          \"description\": \"Specify the interval between keyframes, in seconds or frames, for this output. Default: 12 Related settings: When you specify the GOP size in seconds, set GOP mode control (GopSizeUnits) to Specified, seconds (SECONDS). The default value for GOP mode control (GopSizeUnits) is Frames (FRAMES).\"\n        }\n      ]\n    },\n    \"GopSizeUnits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2GopSizeUnits\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gopSizeUnits\"\n          },\n         \
  \ \"description\": \"Specify the units for GOP size (GopSize). If you don't specify a value here, by default the encoder measures GOP size in frames.\"\n        }\n      ]\n    },\n    \"HrdBufferFinalFillPercentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max100\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hrdBufferFinalFillPercentage\"\n          },\n          \"description\": \"If your downstream systems have strict buffer requirements: Specify the minimum percentage of the HRD buffer that's available at the end of each encoded video segment. For the best video quality: Set to 0 or leave blank to automatically determine the final buffer fill percentage.\"\n        }\n      ]\n    },\n    \"HrdBufferInitialFillPercentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max100\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hrdBufferInitialFillPercentage\"\
  \n          },\n          \"description\": \"Percentage of the buffer that should initially be filled (HRD buffer model).\"\n        }\n      ]\n    },\n    \"HrdBufferSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max47185920\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hrdBufferSize\"\n          },\n          \"description\": \"Size of buffer (HRD buffer model) in bits. For example, enter five megabits as 5000000.\"\n        }\n      ]\n    },\n    \"InterlaceMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2InterlaceMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"interlaceMode\"\n          },\n          \"description\": \"Choose the scan line type for the output. Keep the default value, Progressive (PROGRESSIVE) to create a progressive output, regardless of the scan type of your input. Use Top field first (TOP_FIELD) or Bottom field first\
  \ (BOTTOM_FIELD) to create an output that's interlaced with the same field polarity throughout. Use Follow, default top (FOLLOW_TOP_FIELD) or Follow, default bottom (FOLLOW_BOTTOM_FIELD) to produce outputs with the same field polarity as the source. For jobs that have multiple inputs, the output field polarity might change over the course of the output. Follow behavior depends on the input scan type. If the source is interlaced, the output will be interlaced with the same polarity as the source. If the source is progressive, the output will be interlaced with top field bottom field first, depending on which of the Follow options you choose.\"\n        }\n      ]\n    },\n    \"IntraDcPrecision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2IntraDcPrecision\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"intraDcPrecision\"\n          },\n          \"description\": \"Use Intra DC precision (Mpeg2IntraDcPrecision) to set quantization\
  \ precision for intra-block DC coefficients. If you choose the value auto, the service will automatically select the precision based on the per-frame compression ratio.\"\n        }\n      ]\n    },\n    \"MaxBitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1000Max300000000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxBitrate\"\n          },\n          \"description\": \"Maximum bitrate in bits/second. For example, enter five megabits per second as 5000000.\"\n        }\n      ]\n    },\n    \"MinIInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max30\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"minIInterval\"\n          },\n          \"description\": \"Use this setting only when you also enable Scene change detection (SceneChangeDetect). This setting determines how the encoder manages the spacing between I-frames that it inserts\
  \ as part of the I-frame cadence and the I-frames that it inserts for Scene change detection. When you specify a value for this setting, the encoder determines whether to skip a cadence-driven I-frame by the value you set. For example, if you set Min I interval (minIInterval) to 5 and a cadence-driven I-frame would fall within 5 frames of a scene-change I-frame, then the encoder skips the cadence-driven I-frame. In this way, one GOP is shrunk slightly and one GOP is stretched slightly. When the cadence-driven I-frames are farther from the scene-change I-frame than the value you set, then the encoder leaves all I-frames in place and the GOPs surrounding the scene change are smaller than the usual cadence GOPs.\"\n        }\n      ]\n    },\n    \"NumberBFramesBetweenReferenceFrames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max7\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"numberBFramesBetweenReferenceFrames\"\n\
  \          },\n          \"description\": \"Specify the number of B-frames that MediaConvert puts between reference frames in this output. Valid values are whole numbers from 0 through 7. When you don't specify a value, MediaConvert defaults to 2.\"\n        }\n      ]\n    },\n    \"ParControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2ParControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"parControl\"\n          },\n          \"description\": \"Optional. Specify how the service determines the pixel aspect ratio (PAR) for this output. The default behavior, Follow source (INITIALIZE_FROM_SOURCE), uses the PAR from your input video for your output. To specify a different PAR in the console, choose any value other than Follow source. To specify a different PAR by editing the JSON job specification, choose SPECIFIED. When you choose SPECIFIED for this setting, you must also specify values for the parNumerator and parDenominator\
  \ settings.\"\n        }\n      ]\n    },\n    \"ParDenominator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"parDenominator\"\n          },\n          \"description\": \"Required when you set Pixel aspect ratio (parControl) to SPECIFIED. On the console, this corresponds to any value other than Follow source. When you specify an output pixel aspect ratio (PAR) that is different from your input video PAR, provide your output PAR as a ratio. For example, for D1/DV NTSC widescreen, you would specify the ratio 40:33. In this example, the value for parDenominator is 33.\"\n        }\n      ]\n    },\n    \"ParNumerator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"parNumerator\"\n          },\n          \"description\": \"Required\
  \ when you set Pixel aspect ratio (parControl) to SPECIFIED. On the console, this corresponds to any value other than Follow source. When you specify an output pixel aspect ratio (PAR) that is different from your input video PAR, provide your output PAR as a ratio. For example, for D1/DV NTSC widescreen, you would specify the ratio 40:33. In this example, the value for parNumerator is 40.\"\n        }\n      ]\n    },\n    \"QualityTuningLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2QualityTuningLevel\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"qualityTuningLevel\"\n          },\n          \"description\": \"Optional. Use Quality tuning level (qualityTuningLevel) to choose how you want to trade off encoding speed for output video quality. The default behavior is faster, lower quality, single-pass encoding.\"\n        }\n      ]\n    },\n    \"RateControlMode\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/Mpeg2RateControlMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"rateControlMode\"\n          },\n          \"description\": \"Use Rate control mode (Mpeg2RateControlMode) to specify whether the bitrate is variable (vbr) or constant (cbr).\"\n        }\n      ]\n    },\n    \"ScanTypeConversionMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2ScanTypeConversionMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scanTypeConversionMode\"\n          },\n          \"description\": \"Use this setting for interlaced outputs, when your output frame rate is half of your input frame rate. In this situation, choose Optimized interlacing (INTERLACED_OPTIMIZE) to create a better quality interlaced output. In this case, each progressive frame from the input corresponds to an interlaced field in the output. Keep the default value, Basic interlacing (INTERLACED), for all other output\
  \ frame rates. With basic interlacing, MediaConvert performs any frame rate conversion first and then interlaces the frames. When you choose Optimized interlacing and you set your output frame rate to a value that isn't suitable for optimized interlacing, MediaConvert automatically falls back to basic interlacing. Required settings: To use optimized interlacing, you must set Telecine (telecine) to None (NONE) or Soft (SOFT). You can't use optimized interlacing for hard telecine outputs. You must also set Interlace mode (interlaceMode) to a value other than Progressive (PROGRESSIVE).\"\n        }\n      ]\n    },\n    \"SceneChangeDetect\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2SceneChangeDetect\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sceneChangeDetect\"\n          },\n          \"description\": \"Enable this setting to insert I-frames at scene changes that the service automatically detects. This improves video\
  \ quality and is enabled by default.\"\n        }\n      ]\n    },\n    \"SlowPal\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2SlowPal\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"slowPal\"\n          },\n          \"description\": \"Ignore this setting unless your input frame rate is 23.976 or 24 frames per second (fps). Enable slow PAL to create a 25 fps output. When you enable slow PAL, MediaConvert relabels the video frames to 25 fps and resamples your audio to keep it synchronized with the video. Note that enabling this setting will slightly reduce the duration of your video. Required settings: You must also set Framerate to 25. In your JSON job specification, set (framerateControl) to (SPECIFIED), (framerateNumerator) to 25 and (framerateDenominator) to 1.\"\n        }\n      ]\n    },\n    \"Softness\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max128\"\n        },\n\
  \        {\n          \"xml\": {\n            \"name\": \"softness\"\n          },\n          \"description\": \"Ignore this setting unless you need to comply with a specification that requires a specific value. If you don't have a specification requirement, we recommend that you adjust the softness of your output by using a lower value for the setting Sharpness (sharpness) or by enabling a noise reducer filter (noiseReducerFilter). The Softness (softness) setting specifies the quantization matrices that the encoder uses. Keep the default value, 0, to use the AWS Elemental default matrices. Choose a value from 17 to 128 to use planar interpolation. Increasing values from 17 to 128 result in increasing reduction of high-frequency data. The value 128 results in the softest video.\"\n        }\n      ]\n    },\n    \"SpatialAdaptiveQuantization\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2SpatialAdaptiveQuantization\"\n        },\n        {\n      \
  \    \"xml\": {\n            \"name\": \"spatialAdaptiveQuantization\"\n          },\n          \"description\": \"Keep the default value, Enabled (ENABLED), to adjust quantization within each frame based on spatial variation of content complexity. When you enable this feature, the encoder uses fewer bits on areas that can sustain more distortion with no noticeable visual degradation and uses more bits on areas where any small distortion will be noticeable. For example, complex textured blocks are encoded with fewer bits and smooth textured blocks are encoded with more bits. Enabling this feature will almost always improve your video quality. Note, though, that this feature doesn't take into account where the viewer's attention is likely to be. If viewers are likely to be focusing their attention on a part of the screen with a lot of complex texture, you might choose to disable this feature. Related setting: When you enable spatial adaptive quantization, set the value for Adaptive quantization\
  \ (adaptiveQuantization) depending on your content. For homogeneous content, such as cartoons and video games, set it to Low. For content with a wider variety of textures, set it to High or Higher.\"\n        }\n      ]\n    },\n    \"Syntax\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2Syntax\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"syntax\"\n          },\n          \"description\": \"Specify whether this output's video uses the D10 syntax. Keep the default value to not use the syntax. Related settings: When you choose D10 (D_10) for your MXF profile (profile), you must also set this value to D10 (D_10).\"\n        }\n      ]\n    },\n    \"Telecine\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2Telecine\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"telecine\"\n          },\n          \"description\": \"When you do frame rate conversion from 23.976 frames\
  \ per second (fps) to 29.97 fps, and your output scan type is interlaced, you can optionally enable hard or soft telecine to create a smoother picture. Hard telecine (HARD) produces a 29.97i output. Soft telecine (SOFT) produces an output with a 23.976 output that signals to the video player device to do the conversion during play back. When you keep the default value, None (NONE), MediaConvert does a standard frame rate conversion to 29.97 without doing anything with the field polarity to create a smoother picture.\"\n        }\n      ]\n    },\n    \"TemporalAdaptiveQuantization\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2TemporalAdaptiveQuantization\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"temporalAdaptiveQuantization\"\n          },\n          \"description\": \"Keep the default value, Enabled (ENABLED), to adjust quantization within each frame based on temporal variation of content complexity. When you enable\
  \ this feature, the encoder uses fewer bits on areas of the frame that aren't moving and uses more bits on complex objects with sharp edges that move a lot. For example, this feature improves the readability of text tickers on newscasts and scoreboards on sports matches. Enabling this feature will almost always improve your video quality. Note, though, that this feature doesn't take into account where the viewer's attention is likely to be. If viewers are likely to be focusing their attention on a part of the screen that doesn't have moving objects with sharp edges, such as sports athletes' faces, you might choose to disable this feature. Related setting: When you enable temporal quantization, adjust the strength of the filter with the setting Adaptive quantization (adaptiveQuantization).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mpeg2-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Mpeg2Settings
---
