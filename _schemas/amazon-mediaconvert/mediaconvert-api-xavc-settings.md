---
description: Required when you set (Codec) under (VideoDescription)>(CodecSettings) to the value XAVC.
layout: schema
name: XavcSettings
properties_list:
- description: ''
  name: AdaptiveQuantization
  type: object
- description: ''
  name: EntropyEncoding
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
  name: Profile
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
  name: TemporalAdaptiveQuantization
  type: object
- description: ''
  name: Xavc4kIntraCbgProfileSettings
  type: object
- description: ''
  name: Xavc4kIntraVbrProfileSettings
  type: object
- description: ''
  name: Xavc4kProfileSettings
  type: object
- description: ''
  name: XavcHdIntraCbgProfileSettings
  type: object
- description: ''
  name: XavcHdProfileSettings
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-xavc-settings-schema.json
slug: mediaconvert-api-xavc-settings
source_filename: mediaconvert-api-xavc-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-xavc-settings-schema.json\",\n  \"title\": \"XavcSettings\",\n  \"description\": \"Required when you set (Codec) under (VideoDescription)>(CodecSettings) to the value XAVC.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdaptiveQuantization\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XavcAdaptiveQuantization\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"adaptiveQuantization\"\n          },\n          \"description\": \"Keep the default value, Auto (AUTO), for this setting to have MediaConvert automatically apply the best types of quantization for your video content. When you want to apply your quantization settings manually, you must set Adaptive quantization (adaptiveQuantization) to a value other than Auto (AUTO).\
  \ Use this setting to specify the strength of any adaptive quantization filters that you enable. If you don't want MediaConvert to do any adaptive quantization in this transcode, set Adaptive quantization to Off (OFF). Related settings: The value that you choose here applies to the following settings: Flicker adaptive quantization (flickerAdaptiveQuantization), Spatial adaptive quantization (spatialAdaptiveQuantization), and Temporal adaptive quantization (temporalAdaptiveQuantization).\"\n        }\n      ]\n    },\n    \"EntropyEncoding\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XavcEntropyEncoding\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"entropyEncoding\"\n          },\n          \"description\": \"Optional. Choose a specific entropy encoding mode only when you want to override XAVC recommendations. If you choose the value auto, MediaConvert uses the mode that the XAVC file format specifies given this output's operating\
  \ point.\"\n        }\n      ]\n    },\n    \"FramerateControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XavcFramerateControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateControl\"\n          },\n          \"description\": \"If you are using the console, use the Frame rate setting to specify the frame rate for this output. If you want to keep the same frame rate as the input video, choose Follow source. If you want to do frame rate conversion, choose a frame rate from the dropdown list. The framerates shown in the dropdown list are decimal approximations of fractions. If you are creating your transcoding job specification as a JSON file without the console, use FramerateControl to specify which value the service uses for the frame rate for this output. Choose INITIALIZE_FROM_SOURCE if you want the service to use the frame rate from the input. Choose SPECIFIED if you want the service to use the frame rate that you\
  \ specify in the settings FramerateNumerator and FramerateDenominator.\"\n        }\n      ]\n    },\n    \"FramerateConversionAlgorithm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XavcFramerateConversionAlgorithm\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateConversionAlgorithm\"\n          },\n          \"description\": \"Choose the method that you want MediaConvert to use when increasing or decreasing the frame rate. We recommend using drop duplicate (DUPLICATE_DROP) for numerically simple conversions, such as 60 fps to 30 fps. For numerically complex conversions, you can use interpolate (INTERPOLATE) to avoid stutter. This results in a smooth picture, but might introduce undesirable video artifacts. For complex frame rate conversions, especially if your source video has already been converted from its original cadence, use FrameFormer (FRAMEFORMER) to do motion-compensated interpolation. FrameFormer chooses the\
  \ best conversion method frame by frame. Note that using FrameFormer increases the transcoding time and incurs a significant add-on cost.\"\n        }\n      ]\n    },\n    \"FramerateDenominator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max1001\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateDenominator\"\n          },\n          \"description\": \"When you use the API for transcode jobs that use frame rate conversion, specify the frame rate as a fraction. For example, 24000 / 1001 = 23.976 fps. Use FramerateDenominator to specify the denominator of this fraction. In this example, use 1001 for the value of FramerateDenominator. When you use the console for transcode jobs that use frame rate conversion, provide the value as a decimal number for Frame rate. In this example, specify 23.976.\"\n        }\n      ]\n    },\n    \"FramerateNumerator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/__integerMin24Max60000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateNumerator\"\n          },\n          \"description\": \"When you use the API for transcode jobs that use frame rate conversion, specify the frame rate as a fraction. For example, 24000 / 1001 = 23.976 fps. Use FramerateNumerator to specify the numerator of this fraction. In this example, use 24000 for the value of FramerateNumerator. When you use the console for transcode jobs that use frame rate conversion, provide the value as a decimal number for Framerate. In this example, specify 23.976.\"\n        }\n      ]\n    },\n    \"Profile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XavcProfile\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"profile\"\n          },\n          \"description\": \"Specify the XAVC profile for this output. For more information, see the Sony documentation at https://www.xavc-info.org/.\
  \ Note that MediaConvert doesn't support the interlaced video XAVC operating points for XAVC_HD_INTRA_CBG. To create an interlaced XAVC output, choose the profile XAVC_HD.\"\n        }\n      ]\n    },\n    \"SlowPal\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XavcSlowPal\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"slowPal\"\n          },\n          \"description\": \"Ignore this setting unless your input frame rate is 23.976 or 24 frames per second (fps). Enable slow PAL to create a 25 fps output by relabeling the video frames and resampling your audio. Note that enabling this setting will slightly reduce the duration of your video. Related settings: You must also set Frame rate to 25. In your JSON job specification, set (framerateControl) to (SPECIFIED), (framerateNumerator) to 25 and (framerateDenominator) to 1.\"\n        }\n      ]\n    },\n    \"Softness\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max128\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"softness\"\n          },\n          \"description\": \"Ignore this setting unless your downstream workflow requires that you specify it explicitly. Otherwise, we recommend that you adjust the softness of your output by using a lower value for the setting Sharpness (sharpness) or by enabling a noise reducer filter (noiseReducerFilter). The Softness (softness) setting specifies the quantization matrices that the encoder uses. Keep the default value, 0, for flat quantization. Choose the value 1 or 16 to use the default JVT softening quantization matricies from the H.264 specification. Choose a value from 17 to 128 to use planar interpolation. Increasing values from 17 to 128 result in increasing reduction of high-frequency data. The value 128 results in the softest video.\"\n        }\n      ]\n    },\n    \"SpatialAdaptiveQuantization\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XavcSpatialAdaptiveQuantization\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"spatialAdaptiveQuantization\"\n          },\n          \"description\": \"The best way to set up adaptive quantization is to keep the default value, Auto (AUTO), for the setting Adaptive quantization (adaptiveQuantization). When you do so, MediaConvert automatically applies the best types of quantization for your video content. Include this setting in your JSON job specification only when you choose to change the default value for Adaptive quantization. For this setting, keep the default value, Enabled (ENABLED), to adjust quantization within each frame based on spatial variation of content complexity. When you enable this feature, the encoder uses fewer bits on areas that can sustain more distortion with no noticeable visual degradation and uses more bits on areas where any small distortion will be noticeable. For example, complex textured blocks are encoded with fewer bits and smooth textured blocks are encoded with\
  \ more bits. Enabling this feature will almost always improve your video quality. Note, though, that this feature doesn't take into account where the viewer's attention is likely to be. If viewers are likely to be focusing their attention on a part of the screen with a lot of complex texture, you might choose to disable this feature. Related setting: When you enable spatial adaptive quantization, set the value for Adaptive quantization (adaptiveQuantization) depending on your content. For homogeneous content, such as cartoons and video games, set it to Low. For content with a wider variety of textures, set it to High or Higher.\"\n        }\n      ]\n    },\n    \"TemporalAdaptiveQuantization\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XavcTemporalAdaptiveQuantization\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"temporalAdaptiveQuantization\"\n          },\n          \"description\": \"The best way to set up adaptive quantization\
  \ is to keep the default value, Auto (AUTO), for the setting Adaptive quantization (adaptiveQuantization). When you do so, MediaConvert automatically applies the best types of quantization for your video content. Include this setting in your JSON job specification only when you choose to change the default value for Adaptive quantization. For this setting, keep the default value, Enabled (ENABLED), to adjust quantization within each frame based on temporal variation of content complexity. When you enable this feature, the encoder uses fewer bits on areas of the frame that aren't moving and uses more bits on complex objects with sharp edges that move a lot. For example, this feature improves the readability of text tickers on newscasts and scoreboards on sports matches. Enabling this feature will almost always improve your video quality. Note, though, that this feature doesn't take into account where the viewer's attention is likely to be. If viewers are likely to be focusing their attention\
  \ on a part of the screen that doesn't have moving objects with sharp edges, such as sports athletes' faces, you might choose to disable this feature. Related setting: When you enable temporal adaptive quantization, adjust the strength of the filter with the setting Adaptive quantization (adaptiveQuantization).\"\n        }\n      ]\n    },\n    \"Xavc4kIntraCbgProfileSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Xavc4kIntraCbgProfileSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"xavc4kIntraCbgProfileSettings\"\n          },\n          \"description\": \"Required when you set (Profile) under (VideoDescription)>(CodecSettings)>(XavcSettings) to the value XAVC_4K_INTRA_CBG.\"\n        }\n      ]\n    },\n    \"Xavc4kIntraVbrProfileSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Xavc4kIntraVbrProfileSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\"\
  : \"xavc4kIntraVbrProfileSettings\"\n          },\n          \"description\": \"Required when you set (Profile) under (VideoDescription)>(CodecSettings)>(XavcSettings) to the value XAVC_4K_INTRA_VBR.\"\n        }\n      ]\n    },\n    \"Xavc4kProfileSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Xavc4kProfileSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"xavc4kProfileSettings\"\n          },\n          \"description\": \"Required when you set (Profile) under (VideoDescription)>(CodecSettings)>(XavcSettings) to the value XAVC_4K.\"\n        }\n      ]\n    },\n    \"XavcHdIntraCbgProfileSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XavcHdIntraCbgProfileSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"xavcHdIntraCbgProfileSettings\"\n          },\n          \"description\": \"Required when you set (Profile) under (VideoDescription)>(CodecSettings)>(XavcSettings)\
  \ to the value XAVC_HD_INTRA_CBG.\"\n        }\n      ]\n    },\n    \"XavcHdProfileSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XavcHdProfileSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"xavcHdProfileSettings\"\n          },\n          \"description\": \"Required when you set (Profile) under (VideoDescription)>(CodecSettings)>(XavcSettings) to the value XAVC_HD.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-xavc-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: XavcSettings
---
