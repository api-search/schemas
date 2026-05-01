---
description: Settings for color correction.
layout: schema
name: ColorCorrector
properties_list:
- description: ''
  name: Brightness
  type: object
- description: ''
  name: ClipLimits
  type: object
- description: ''
  name: ColorSpaceConversion
  type: object
- description: ''
  name: Contrast
  type: object
- description: ''
  name: Hdr10Metadata
  type: object
- description: ''
  name: HdrToSdrToneMapper
  type: object
- description: ''
  name: Hue
  type: object
- description: ''
  name: SampleRangeConversion
  type: object
- description: ''
  name: Saturation
  type: object
- description: ''
  name: SdrReferenceWhiteLevel
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-color-corrector-schema.json
slug: mediaconvert-api-color-corrector
source_filename: mediaconvert-api-color-corrector-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-color-corrector-schema.json\",\n  \"title\": \"ColorCorrector\",\n  \"description\": \"Settings for color correction.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Brightness\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max100\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"brightness\"\n          },\n          \"description\": \"Brightness level.\"\n        }\n      ]\n    },\n    \"ClipLimits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClipLimits\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clipLimits\"\n          },\n          \"description\": \"Specify YUV limits and RGB tolerances when you set Sample range conversion to Limited range\
  \ clip.\"\n        }\n      ]\n    },\n    \"ColorSpaceConversion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ColorSpaceConversion\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"colorSpaceConversion\"\n          },\n          \"description\": \"Specify the color space you want for this output. The service supports conversion between HDR formats, between SDR formats, from SDR to HDR, and from HDR to SDR. SDR to HDR conversion doesn't upgrade the dynamic range. The converted video has an HDR format, but visually appears the same as an unconverted output. HDR to SDR conversion uses tone mapping to approximate the outcome of manually regrading from HDR to SDR. When you specify an output color space, MediaConvert uses the following color space metadata, which includes color primaries, transfer characteristics, and matrix coefficients:\\n  * HDR 10: BT.2020, PQ, BT.2020 non-constant\\n  * HLG 2020: BT.2020, HLG, BT.2020 non-constant\\\
  n  * P3DCI (Theater): DCIP3, SMPTE 428M, BT.709\\n  * P3D65 (SDR): Display P3, sRGB, BT.709\\n  * P3D65 (HDR): Display P3, PQ, BT.709\"\n        }\n      ]\n    },\n    \"Contrast\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max100\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"contrast\"\n          },\n          \"description\": \"Contrast level.\"\n        }\n      ]\n    },\n    \"Hdr10Metadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Hdr10Metadata\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hdr10Metadata\"\n          },\n          \"description\": \"Use these settings when you convert to the HDR 10 color space. Specify the SMPTE ST 2086 Mastering Display Color Volume static metadata that you want signaled in the output. These values don't affect the pixel values that are encoded in the video stream. They are intended to help the downstream video\
  \ player display content in a way that reflects the intentions of the the content creator. When you set Color space conversion (ColorSpaceConversion) to HDR 10 (FORCE_HDR10), these settings are required. You must set values for Max frame average light level (maxFrameAverageLightLevel) and Max content light level (maxContentLightLevel); these settings don't have a default value. The default values for the other HDR 10 metadata settings are defined by the P3D65 color space. For more information about MediaConvert HDR jobs, see https://docs.aws.amazon.com/console/mediaconvert/hdr.\"\n        }\n      ]\n    },\n    \"HdrToSdrToneMapper\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HDRToSDRToneMapper\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hdrToSdrToneMapper\"\n          },\n          \"description\": \"Specify how MediaConvert maps brightness and colors from your HDR input to your SDR output. The mode that you select represents\
  \ a creative choice, with different tradeoffs in the details and tones of your output. To maintain details in bright or saturated areas of your output: Choose Preserve details. For some sources, your SDR output may look less bright and less saturated when compared to your HDR source. MediaConvert automatically applies this mode for HLG sources, regardless of your choice. For a bright and saturated output: Choose Vibrant. We recommend that you choose this mode when any of your source content is HDR10, and for the best results when it is mastered for 1000 nits. You may notice loss of details in bright or saturated areas of your output. HDR to SDR tone mapping has no effect when your input is SDR.\"\n        }\n      ]\n    },\n    \"Hue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMinNegative180Max180\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hue\"\n          },\n          \"description\": \"Hue in degrees.\"\n   \
  \     }\n      ]\n    },\n    \"SampleRangeConversion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SampleRangeConversion\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sampleRangeConversion\"\n          },\n          \"description\": \"Specify how MediaConvert limits the color sample range for this output. To create a limited range output from a full range input: Choose Limited range squeeze. For full range inputs, MediaConvert performs a linear offset to color samples equally across all pixels and frames. Color samples in 10-bit outputs are limited to 64 through 940, and 8-bit outputs are limited to 16 through 235. Note: For limited range inputs, values for color samples are passed through to your output unchanged. MediaConvert does not limit the sample range. To correct pixels in your input that are out of range or out of gamut: Choose Limited range clip. Use for broadcast applications. MediaConvert conforms any pixels outside\
  \ of the values that you specify under Minimum YUV and Maximum YUV to limited range bounds. MediaConvert also corrects any YUV values that, when converted to RGB, would be outside the bounds you specify under Minimum RGB tolerance and Maximum RGB tolerance. With either limited range conversion, MediaConvert writes the sample range metadata in the output.\"\n        }\n      ]\n    },\n    \"Saturation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max100\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"saturation\"\n          },\n          \"description\": \"Saturation level.\"\n        }\n      ]\n    },\n    \"SdrReferenceWhiteLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin100Max1000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sdrReferenceWhiteLevel\"\n          },\n          \"description\": \"Specify the reference white level, in nits,\
  \ for all of your SDR inputs. Use to correct brightness levels within HDR10 outputs. The following color metadata must be present in your SDR input: color primaries, transfer characteristics, and matrix coefficients. If your SDR input has missing color metadata, or if you want to correct input color metadata, manually specify a color space in the input video selector. For 1,000 nit peak brightness displays, we recommend that you set SDR reference white level to 203 (according to ITU-R BT.2408). Leave blank to use the default value of 100, or specify an integer from 100 to 1000.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-color-corrector-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ColorCorrector
---
