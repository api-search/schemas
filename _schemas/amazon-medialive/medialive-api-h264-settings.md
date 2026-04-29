---
description: H264 Settings
layout: schema
name: H264Settings
properties_list:
- description: ''
  name: AdaptiveQuantization
  type: object
- description: ''
  name: AfdSignaling
  type: object
- description: ''
  name: Bitrate
  type: object
- description: ''
  name: BufFillPct
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
  name: EntropyEncoding
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
  name: ForceFieldPictures
  type: object
- description: ''
  name: FramerateControl
  type: object
- description: ''
  name: FramerateDenominator
  type: object
- description: ''
  name: FramerateNumerator
  type: object
- description: ''
  name: GopBReference
  type: object
- description: ''
  name: GopClosedCadence
  type: object
- description: ''
  name: GopNumBFrames
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
  name: NumRefFrames
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
  name: Profile
  type: object
- description: ''
  name: QualityLevel
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
  name: Softness
  type: object
- description: ''
  name: SpatialAq
  type: object
- description: ''
  name: SubgopLength
  type: object
- description: ''
  name: Syntax
  type: object
- description: ''
  name: TemporalAq
  type: object
- description: ''
  name: TimecodeInsertion
  type: object
- description: ''
  name: TimecodeBurninSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-h264-settings-schema.json
slug: medialive-api-h264-settings
source_filename: medialive-api-h264-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-h264-settings-schema.json\",\n  \"title\": \"H264Settings\",\n  \"description\": \"H264 Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdaptiveQuantization\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H264AdaptiveQuantization\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"adaptiveQuantization\"\n          },\n          \"description\": \"Enables or disables adaptive quantization, which is a technique MediaLive can apply to video on a frame-by-frame basis to produce more compression without losing quality. There are three types of adaptive quantization: flicker, spatial, and temporal. Set the field in one of these ways: Set to Auto. Recommended. For each type of AQ, MediaLive will determine if AQ is needed, and\
  \ if so, the appropriate strength. Set a strength (a value other than Auto or Disable). This strength will apply to any of the AQ fields that you choose to enable. Set to Disabled to disable all types of adaptive quantization.\"\n        }\n      ]\n    },\n    \"AfdSignaling\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AfdSignaling\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"afdSignaling\"\n          },\n          \"description\": \"Indicates that AFD values will be written into the output stream.  If afdSignaling is \\\"auto\\\", the system will try to preserve the input AFD value (in cases where multiple AFD values are valid). If set to \\\"fixed\\\", the AFD value will be the value configured in the fixedAfd parameter.\"\n        }\n      ]\n    },\n    \"Bitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1000\"\n        },\n        {\n          \"xml\": {\n            \"\
  name\": \"bitrate\"\n          },\n          \"description\": \"Average bitrate in bits/second. Required when the rate control mode is VBR or CBR. Not used for QVBR. In an MS Smooth output group, each output must have a unique value when its bitrate is rounded down to the nearest multiple of 1000.\"\n        }\n      ]\n    },\n    \"BufFillPct\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max100\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bufFillPct\"\n          },\n          \"description\": \"Percentage of the buffer that should initially be filled (HRD buffer model).\"\n        }\n      ]\n    },\n    \"BufSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bufSize\"\n          },\n          \"description\": \"Size of buffer (HRD buffer model) in bits.\"\n        }\n      ]\n    },\n    \"ColorMetadata\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H264ColorMetadata\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"colorMetadata\"\n          },\n          \"description\": \"Includes colorspace metadata in the output.\"\n        }\n      ]\n    },\n    \"ColorSpaceSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H264ColorSpaceSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"colorSpaceSettings\"\n          },\n          \"description\": \"Color Space settings\"\n        }\n      ]\n    },\n    \"EntropyEncoding\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H264EntropyEncoding\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"entropyEncoding\"\n          },\n          \"description\": \"Entropy encoding mode.  Use cabac (must be in Main or High profile) or cavlc.\"\n        }\n      ]\n    },\n    \"FilterSettings\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H264FilterSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"filterSettings\"\n          },\n          \"description\": \"Optional filters that you can apply to an encode.\"\n        }\n      ]\n    },\n    \"FixedAfd\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FixedAfd\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fixedAfd\"\n          },\n          \"description\": \"Four bit AFD value to write on all frames of video in the output stream. Only valid when afdSignaling is set to 'Fixed'.\"\n        }\n      ]\n    },\n    \"FlickerAq\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H264FlickerAq\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flickerAq\"\n          },\n          \"description\": \"Flicker AQ makes adjustments within each frame to reduce flicker or\
  \ 'pop' on I-frames. The value to enter in this field depends on the value in the Adaptive quantization field: If you have set the Adaptive quantization field to Auto, MediaLive ignores any value in this field. MediaLive will determine if flicker AQ is appropriate and will apply the appropriate strength. If you have set the Adaptive quantization field to a strength, you can set this field to Enabled or Disabled. Enabled: MediaLive will apply flicker AQ using the specified strength. Disabled: MediaLive won't apply flicker AQ. If you have set the Adaptive quantization to Disabled, MediaLive ignores any value in this field and doesn't apply flicker AQ.\"\n        }\n      ]\n    },\n    \"ForceFieldPictures\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H264ForceFieldPictures\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"forceFieldPictures\"\n          },\n          \"description\": \"This setting applies only when scan type is \\\
  \"interlaced.\\\" It controls whether coding is performed on a field basis or on a frame basis. (When the video is progressive, the coding is always performed on a frame basis.)\\nenabled: Force MediaLive to code on a field basis, so that odd and even sets of fields are coded separately.\\ndisabled: Code the two sets of fields separately (on a field basis) or together (on a frame basis using PAFF), depending on what is most appropriate for the content.\"\n        }\n      ]\n    },\n    \"FramerateControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H264FramerateControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateControl\"\n          },\n          \"description\": \"This field indicates how the output video frame rate is specified.  If \\\"specified\\\" is selected then the output video frame rate is determined by framerateNumerator and framerateDenominator, else if \\\"initializeFromSource\\\" is selected then the\
  \ output video frame rate will be set equal to the input video frame rate of the first input.\"\n        }\n      ]\n    },\n    \"FramerateDenominator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateDenominator\"\n          },\n          \"description\": \"Framerate denominator.\"\n        }\n      ]\n    },\n    \"FramerateNumerator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateNumerator\"\n          },\n          \"description\": \"Framerate numerator - framerate is a fraction, e.g. 24000 / 1001 = 23.976 fps.\"\n        }\n      ]\n    },\n    \"GopBReference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H264GopBReference\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gopBReference\"\
  \n          },\n          \"description\": \"Documentation update needed\"\n        }\n      ]\n    },\n    \"GopClosedCadence\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gopClosedCadence\"\n          },\n          \"description\": \"Frequency of closed GOPs. In streaming applications, it is recommended that this be set to 1 so a decoder joining mid-stream will receive an IDR frame as quickly as possible. Setting this value to 0 will break output segmenting.\"\n        }\n      ]\n    },\n    \"GopNumBFrames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max7\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gopNumBFrames\"\n          },\n          \"description\": \"Number of B-frames between reference frames.\"\n        }\n      ]\n    },\n    \"GopSize\": {\n      \"allOf\": [\n        {\n      \
  \    \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gopSize\"\n          },\n          \"description\": \"GOP size (keyframe interval) in units of either frames or seconds per gopSizeUnits.\\nIf gopSizeUnits is frames, gopSize must be an integer and must be greater than or equal to 1.\\nIf gopSizeUnits is seconds, gopSize must be greater than 0, but need not be an integer.\"\n        }\n      ]\n    },\n    \"GopSizeUnits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H264GopSizeUnits\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gopSizeUnits\"\n          },\n          \"description\": \"Indicates if the gopSize is specified in frames or seconds. If seconds the system will convert the gopSize into a frame count at run time.\"\n        }\n      ]\n    },\n    \"Level\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H264Level\"\n   \
  \     },\n        {\n          \"xml\": {\n            \"name\": \"level\"\n          },\n          \"description\": \"H.264 Level.\"\n        }\n      ]\n    },\n    \"LookAheadRateControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H264LookAheadRateControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"lookAheadRateControl\"\n          },\n          \"description\": \"Amount of lookahead. A value of low can decrease latency and memory usage, while high can produce better quality for certain content.\"\n        }\n      ]\n    },\n    \"MaxBitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxBitrate\"\n          },\n          \"description\": \"For QVBR: See the tooltip for Quality level\\n\\nFor VBR: Set the maximum bitrate in order to accommodate expected spikes in the complexity of the video.\"\n\
  \        }\n      ]\n    },\n    \"MinIInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max30\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"minIInterval\"\n          },\n          \"description\": \"Only meaningful if sceneChangeDetect is set to enabled.  Defaults to 5 if multiplex rate control is used.  Enforces separation between repeated (cadence) I-frames and I-frames inserted by Scene Change Detection. If a scene change I-frame is within I-interval frames of a cadence I-frame, the GOP is shrunk and/or stretched to the scene change I-frame. GOP stretch requires enabling lookahead as well as setting I-interval. The normal cadence resumes for the next GOP. Note: Maximum GOP stretch = GOP size + Min-I-interval - 1\"\n        }\n      ]\n    },\n    \"NumRefFrames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max6\"\n        },\n        {\n          \"xml\": {\n\
  \            \"name\": \"numRefFrames\"\n          },\n          \"description\": \"Number of reference frames to use. The encoder may use more than requested if using B-frames and/or interlaced encoding.\"\n        }\n      ]\n    },\n    \"ParControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H264ParControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"parControl\"\n          },\n          \"description\": \"This field indicates how the output pixel aspect ratio is specified.  If \\\"specified\\\" is selected then the output video pixel aspect ratio is determined by parNumerator and parDenominator, else if \\\"initializeFromSource\\\" is selected then the output pixsel aspect ratio will be set equal to the input video pixel aspect ratio of the first input.\"\n        }\n      ]\n    },\n    \"ParDenominator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1\"\n        },\n      \
  \  {\n          \"xml\": {\n            \"name\": \"parDenominator\"\n          },\n          \"description\": \"Pixel Aspect Ratio denominator.\"\n        }\n      ]\n    },\n    \"ParNumerator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"parNumerator\"\n          },\n          \"description\": \"Pixel Aspect Ratio numerator.\"\n        }\n      ]\n    },\n    \"Profile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H264Profile\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"profile\"\n          },\n          \"description\": \"H.264 Profile.\"\n        }\n      ]\n    },\n    \"QualityLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H264QualityLevel\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"qualityLevel\"\n          },\n          \"description\"\
  : \"Leave as STANDARD_QUALITY or choose a different value (which might result in additional costs to run the channel).\\n- ENHANCED_QUALITY: Produces a slightly better video quality without an increase in the bitrate. Has an effect only when the Rate control mode is QVBR or CBR. If this channel is in a MediaLive multiplex, the value must be ENHANCED_QUALITY.\\n- STANDARD_QUALITY: Valid for any Rate control mode.\"\n        }\n      ]\n    },\n    \"QvbrQualityLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max10\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"qvbrQualityLevel\"\n          },\n          \"description\": \"Controls the target quality for the video encode. Applies only when the rate control mode is QVBR. You can set a target quality or you can let MediaLive determine the best quality. To set a target quality, enter values in the QVBR quality level field and the Max bitrate field. Enter values that\
  \ suit your most important viewing devices. Recommended values are:\\n- Primary screen: Quality level: 8 to 10. Max bitrate: 4M\\n- PC or tablet: Quality level: 7. Max bitrate: 1.5M to 3M\\n- Smartphone: Quality level: 6. Max bitrate: 1M to 1.5M\\nTo let MediaLive decide, leave the QVBR quality level field empty, and in Max bitrate enter the maximum rate you want in the video. For more information, see the section called \\\"Video - rate control mode\\\" in the MediaLive user guide\"\n        }\n      ]\n    },\n    \"RateControlMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H264RateControlMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"rateControlMode\"\n          },\n          \"description\": \"Rate control mode.\\n\\nQVBR: Quality will match the specified quality level except when it is constrained by the\\nmaximum bitrate.  Recommended if you or your viewers pay for bandwidth.\\n\\nVBR: Quality and bitrate vary, depending\
  \ on the video complexity. Recommended instead of QVBR\\nif you want to maintain a specific average bitrate over the duration of the channel.\\n\\nCBR: Quality varies, depending on the video complexity. Recommended only if you distribute\\nyour assets to devices that cannot handle variable bitrates.\\n\\nMultiplex: This rate control mode is only supported (and is required) when the video is being\\ndelivered to a MediaLive Multiplex in which case the rate control configuration is controlled\\nby the properties within the Multiplex Program.\"\n        }\n      ]\n    },\n    \"ScanType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H264ScanType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scanType\"\n          },\n          \"description\": \"Sets the scan type of the output to progressive or top-field-first interlaced.\"\n        }\n      ]\n    },\n    \"SceneChangeDetect\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/H264SceneChangeDetect\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sceneChangeDetect\"\n          },\n          \"description\": \"Scene change detection.\\n\\n- On: inserts I-frames when scene change is detected.\\n- Off: does not force an I-frame when scene change is detected.\"\n        }\n      ]\n    },\n    \"Slices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max32\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"slices\"\n          },\n          \"description\": \"Number of slices per picture. Must be less than or equal to the number of macroblock rows for progressive pictures, and less than or equal to half the number of macroblock rows for interlaced pictures.\\nThis field is optional; when no value is specified the encoder will choose the number of slices based on encode resolution.\"\n        }\n      ]\n    },\n    \"Softness\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max128\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"softness\"\n          },\n          \"description\": \"Softness. Selects quantizer matrix, larger values reduce high-frequency content in the encoded image.  If not set to zero, must be greater than 15.\"\n        }\n      ]\n    },\n    \"SpatialAq\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H264SpatialAq\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"spatialAq\"\n          },\n          \"description\": \"Spatial AQ makes adjustments within each frame based on spatial variation of content complexity. The value to enter in this field depends on the value in the Adaptive quantization field: If you have set the Adaptive quantization field to Auto, MediaLive ignores any value in this field. MediaLive will determine if spatial AQ is appropriate and will apply the appropriate strength.\
  \ If you have set the Adaptive quantization field to a strength, you can set this field to Enabled or Disabled. Enabled: MediaLive will apply spatial AQ using the specified strength. Disabled: MediaLive won't apply spatial AQ. If you have set the Adaptive quantization to Disabled, MediaLive ignores any value in this field and doesn't apply spatial AQ.\"\n        }\n      ]\n    },\n    \"SubgopLength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H264SubGopLength\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"subgopLength\"\n          },\n          \"description\": \"If set to fixed, use gopNumBFrames B-frames per sub-GOP. If set to dynamic, optimize the number of B-frames used for each sub-GOP to improve visual quality.\"\n        }\n      ]\n    },\n    \"Syntax\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H264Syntax\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"syntax\"\
  \n          },\n          \"description\": \"Produces a bitstream compliant with SMPTE RP-2027.\"\n        }\n      ]\n    },\n    \"TemporalAq\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H264TemporalAq\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"temporalAq\"\n          },\n          \"description\": \"Temporal makes adjustments within each frame based on temporal variation of content complexity. The value to enter in this field depends on the value in the Adaptive quantization field: If you have set the Adaptive quantization field to Auto, MediaLive ignores any value in this field. MediaLive will determine if temporal AQ is appropriate and will apply the appropriate strength. If you have set the Adaptive quantization field to a strength, you can set this field to Enabled or Disabled. Enabled: MediaLive will apply temporal AQ using the specified strength. Disabled: MediaLive won't apply temporal AQ. If you have set the Adaptive\
  \ quantization to Disabled, MediaLive ignores any value in this field and doesn't apply temporal AQ.\"\n        }\n      ]\n    },\n    \"TimecodeInsertion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H264TimecodeInsertionBehavior\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timecodeInsertion\"\n          },\n          \"description\": \"Determines how timecodes should be inserted into the video elementary stream.\\n- 'disabled': Do not include timecodes\\n- 'picTimingSei': Pass through picture timing SEI messages from the source specified in Timecode Config\"\n        }\n      ]\n    },\n    \"TimecodeBurninSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimecodeBurninSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timecodeBurninSettings\"\n          },\n          \"description\": \"Timecode burn-in settings\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-h264-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: H264Settings
---
