---
description: H265 Settings
layout: schema
name: H265Settings
properties_list:
- description: ''
  name: AdaptiveQuantization
  type: object
- description: ''
  name: AfdSignaling
  type: object
- description: ''
  name: AlternativeTransferFunction
  type: object
- description: ''
  name: Bitrate
  type: object
- description: ''
  name: BufSize
  type: object
- description: ''
  name: ColorMetadata
  type: object
- description: ''
  name: ColorSpaceSettings
  type: object
- description: ''
  name: FilterSettings
  type: object
- description: ''
  name: FixedAfd
  type: object
- description: ''
  name: FlickerAq
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
  name: Level
  type: object
- description: ''
  name: LookAheadRateControl
  type: object
- description: ''
  name: MaxBitrate
  type: object
- description: ''
  name: MinIInterval
  type: object
- description: ''
  name: ParDenominator
  type: object
- description: ''
  name: ParNumerator
  type: object
- description: ''
  name: Profile
  type: object
- description: ''
  name: QvbrQualityLevel
  type: object
- description: ''
  name: RateControlMode
  type: object
- description: ''
  name: ScanType
  type: object
- description: ''
  name: SceneChangeDetect
  type: object
- description: ''
  name: Slices
  type: object
- description: ''
  name: Tier
  type: object
- description: ''
  name: TimecodeInsertion
  type: object
- description: ''
  name: TimecodeBurninSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-h265-settings-schema.json
slug: medialive-api-h265-settings
source_filename: medialive-api-h265-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-h265-settings-schema.json\",\n  \"title\": \"H265Settings\",\n  \"description\": \"H265 Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdaptiveQuantization\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H265AdaptiveQuantization\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"adaptiveQuantization\"\n          },\n          \"description\": \"Adaptive quantization. Allows intra-frame quantizers to vary to improve visual quality.\"\n        }\n      ]\n    },\n    \"AfdSignaling\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AfdSignaling\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"afdSignaling\"\n          },\n          \"description\": \"Indicates that AFD\
  \ values will be written into the output stream.  If afdSignaling is \\\"auto\\\", the system will try to preserve the input AFD value (in cases where multiple AFD values are valid). If set to \\\"fixed\\\", the AFD value will be the value configured in the fixedAfd parameter.\"\n        }\n      ]\n    },\n    \"AlternativeTransferFunction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H265AlternativeTransferFunction\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"alternativeTransferFunction\"\n          },\n          \"description\": \"Whether or not EML should insert an Alternative Transfer Function SEI message to support backwards compatibility with non-HDR decoders and displays.\"\n        }\n      ]\n    },\n    \"Bitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin100000Max40000000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bitrate\"\n          },\n\
  \          \"description\": \"Average bitrate in bits/second. Required when the rate control mode is VBR or CBR. Not used for QVBR. In an MS Smooth output group, each output must have a unique value when its bitrate is rounded down to the nearest multiple of 1000.\"\n        }\n      ]\n    },\n    \"BufSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin100000Max80000000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bufSize\"\n          },\n          \"description\": \"Size of buffer (HRD buffer model) in bits.\"\n        }\n      ]\n    },\n    \"ColorMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H265ColorMetadata\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"colorMetadata\"\n          },\n          \"description\": \"Includes colorspace metadata in the output.\"\n        }\n      ]\n    },\n    \"ColorSpaceSettings\": {\n      \"allOf\": [\n   \
  \     {\n          \"$ref\": \"#/components/schemas/H265ColorSpaceSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"colorSpaceSettings\"\n          },\n          \"description\": \"Color Space settings\"\n        }\n      ]\n    },\n    \"FilterSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H265FilterSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"filterSettings\"\n          },\n          \"description\": \"Optional filters that you can apply to an encode.\"\n        }\n      ]\n    },\n    \"FixedAfd\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FixedAfd\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fixedAfd\"\n          },\n          \"description\": \"Four bit AFD value to write on all frames of video in the output stream. Only valid when afdSignaling is set to 'Fixed'.\"\n        }\n      ]\n    },\n    \"FlickerAq\":\
  \ {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H265FlickerAq\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flickerAq\"\n          },\n          \"description\": \"If set to enabled, adjust quantization within each frame to reduce flicker or 'pop' on I-frames.\"\n        }\n      ]\n    },\n    \"FramerateDenominator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max3003\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateDenominator\"\n          },\n          \"description\": \"Framerate denominator.\"\n        }\n      ]\n    },\n    \"FramerateNumerator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateNumerator\"\n          },\n          \"description\": \"Framerate numerator - framerate is a fraction, e.g. 24000 / 1001 = 23.976\
  \ fps.\"\n        }\n      ]\n    },\n    \"GopClosedCadence\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gopClosedCadence\"\n          },\n          \"description\": \"Frequency of closed GOPs. In streaming applications, it is recommended that this be set to 1 so a decoder joining mid-stream will receive an IDR frame as quickly as possible. Setting this value to 0 will break output segmenting.\"\n        }\n      ]\n    },\n    \"GopSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gopSize\"\n          },\n          \"description\": \"GOP size (keyframe interval) in units of either frames or seconds per gopSizeUnits.\\nIf gopSizeUnits is frames, gopSize must be an integer and must be greater than or equal to 1.\\nIf gopSizeUnits is seconds, gopSize must\
  \ be greater than 0, but need not be an integer.\"\n        }\n      ]\n    },\n    \"GopSizeUnits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H265GopSizeUnits\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gopSizeUnits\"\n          },\n          \"description\": \"Indicates if the gopSize is specified in frames or seconds. If seconds the system will convert the gopSize into a frame count at run time.\"\n        }\n      ]\n    },\n    \"Level\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H265Level\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"level\"\n          },\n          \"description\": \"H.265 Level.\"\n        }\n      ]\n    },\n    \"LookAheadRateControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H265LookAheadRateControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"lookAheadRateControl\"\n    \
  \      },\n          \"description\": \"Amount of lookahead. A value of low can decrease latency and memory usage, while high can produce better quality for certain content.\"\n        }\n      ]\n    },\n    \"MaxBitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin100000Max40000000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxBitrate\"\n          },\n          \"description\": \"For QVBR: See the tooltip for Quality level\"\n        }\n      ]\n    },\n    \"MinIInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max30\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"minIInterval\"\n          },\n          \"description\": \"Only meaningful if sceneChangeDetect is set to enabled.  Defaults to 5 if multiplex rate control is used.  Enforces separation between repeated (cadence) I-frames and I-frames inserted by Scene Change Detection. If\
  \ a scene change I-frame is within I-interval frames of a cadence I-frame, the GOP is shrunk and/or stretched to the scene change I-frame. GOP stretch requires enabling lookahead as well as setting I-interval. The normal cadence resumes for the next GOP. Note: Maximum GOP stretch = GOP size + Min-I-interval - 1\"\n        }\n      ]\n    },\n    \"ParDenominator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"parDenominator\"\n          },\n          \"description\": \"Pixel Aspect Ratio denominator.\"\n        }\n      ]\n    },\n    \"ParNumerator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"parNumerator\"\n          },\n          \"description\": \"Pixel Aspect Ratio numerator.\"\n        }\n      ]\n    },\n    \"Profile\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/H265Profile\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"profile\"\n          },\n          \"description\": \"H.265 Profile.\"\n        }\n      ]\n    },\n    \"QvbrQualityLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max10\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"qvbrQualityLevel\"\n          },\n          \"description\": \"Controls the target quality for the video encode. Applies only when the rate control mode is QVBR. Set values for the QVBR quality level field and Max bitrate field that suit your most important viewing devices. Recommended values are:\\n- Primary screen: Quality level: 8 to 10. Max bitrate: 4M\\n- PC or tablet: Quality level: 7. Max bitrate: 1.5M to 3M\\n- Smartphone: Quality level: 6. Max bitrate: 1M to 1.5M\"\n        }\n      ]\n    },\n    \"RateControlMode\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/H265RateControlMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"rateControlMode\"\n          },\n          \"description\": \"Rate control mode.\\n\\nQVBR: Quality will match the specified quality level except when it is constrained by the\\nmaximum bitrate.  Recommended if you or your viewers pay for bandwidth.\\n\\nCBR: Quality varies, depending on the video complexity. Recommended only if you distribute\\nyour assets to devices that cannot handle variable bitrates.\\n\\nMultiplex: This rate control mode is only supported (and is required) when the video is being\\ndelivered to a MediaLive Multiplex in which case the rate control configuration is controlled\\nby the properties within the Multiplex Program.\"\n        }\n      ]\n    },\n    \"ScanType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H265ScanType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"\
  scanType\"\n          },\n          \"description\": \"Sets the scan type of the output to progressive or top-field-first interlaced.\"\n        }\n      ]\n    },\n    \"SceneChangeDetect\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H265SceneChangeDetect\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sceneChangeDetect\"\n          },\n          \"description\": \"Scene change detection.\"\n        }\n      ]\n    },\n    \"Slices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max16\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"slices\"\n          },\n          \"description\": \"Number of slices per picture. Must be less than or equal to the number of macroblock rows for progressive pictures, and less than or equal to half the number of macroblock rows for interlaced pictures.\\nThis field is optional; when no value is specified the encoder will choose the\
  \ number of slices based on encode resolution.\"\n        }\n      ]\n    },\n    \"Tier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H265Tier\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tier\"\n          },\n          \"description\": \"H.265 Tier.\"\n        }\n      ]\n    },\n    \"TimecodeInsertion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H265TimecodeInsertionBehavior\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timecodeInsertion\"\n          },\n          \"description\": \"Determines how timecodes should be inserted into the video elementary stream.\\n- 'disabled': Do not include timecodes\\n- 'picTimingSei': Pass through picture timing SEI messages from the source specified in Timecode Config\"\n        }\n      ]\n    },\n    \"TimecodeBurninSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimecodeBurninSettings\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"timecodeBurninSettings\"\n          },\n          \"description\": \"Timecode burn-in settings\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FramerateNumerator\",\n    \"FramerateDenominator\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-h265-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: H265Settings
---
