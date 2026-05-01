---
description: Mpeg2 Settings
layout: schema
name: Mpeg2Settings
properties_list:
- description: ''
  name: AdaptiveQuantization
  type: object
- description: ''
  name: AfdSignaling
  type: object
- description: ''
  name: ColorMetadata
  type: object
- description: ''
  name: ColorSpace
  type: object
- description: ''
  name: DisplayAspectRatio
  type: object
- description: ''
  name: FilterSettings
  type: object
- description: ''
  name: FixedAfd
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
  name: GopNumBFrames
  type: object
- description: ''
  name: GopSize
  type: object
- description: ''
  name: GopSizeUnits
  type: object
- description: ''
  name: ScanType
  type: object
- description: ''
  name: SubgopLength
  type: object
- description: ''
  name: TimecodeInsertion
  type: object
- description: ''
  name: TimecodeBurninSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-mpeg2-settings-schema.json
slug: medialive-api-mpeg2-settings
source_filename: medialive-api-mpeg2-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-mpeg2-settings-schema.json\",\n  \"title\": \"Mpeg2Settings\",\n  \"description\": \"Mpeg2 Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdaptiveQuantization\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2AdaptiveQuantization\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"adaptiveQuantization\"\n          },\n          \"description\": \"Choose Off to disable adaptive quantization. Or choose another value to enable the quantizer and set its strength. The strengths are: Auto, Off, Low, Medium, High. When you enable this field, MediaLive allows intra-frame quantizers to vary, which might improve visual quality.\"\n        }\n      ]\n    },\n    \"AfdSignaling\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/AfdSignaling\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"afdSignaling\"\n          },\n          \"description\": \"Indicates the AFD values that MediaLive will write into the video encode. If you do not know what AFD signaling is, or if your downstream system has not given you guidance, choose AUTO.\\nAUTO: MediaLive will try to preserve the input AFD value (in cases where multiple AFD values are valid).\\nFIXED: MediaLive will use the value you specify in fixedAFD.\"\n        }\n      ]\n    },\n    \"ColorMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2ColorMetadata\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"colorMetadata\"\n          },\n          \"description\": \"Specifies whether to include the color space metadata. The metadata describes the color space that applies to the video (the colorSpace field). We recommend that you insert the metadata.\"\
  \n        }\n      ]\n    },\n    \"ColorSpace\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2ColorSpace\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"colorSpace\"\n          },\n          \"description\": \"Choose the type of color space conversion to apply to the output. For detailed information on setting up both the input and the output to obtain the desired color space in the output, see the section on \\\\\\\"MediaLive Features - Video - color space\\\\\\\" in the MediaLive User Guide.\\nPASSTHROUGH: Keep the color space of the input content - do not convert it.\\nAUTO:Convert all content that is SD to rec 601, and convert all content that is HD to rec 709.\"\n        }\n      ]\n    },\n    \"DisplayAspectRatio\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2DisplayRatio\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"displayAspectRatio\"\n          },\n \
  \         \"description\": \"Sets the pixel aspect ratio for the encode.\"\n        }\n      ]\n    },\n    \"FilterSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2FilterSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"filterSettings\"\n          },\n          \"description\": \"Optionally specify a noise reduction filter, which can improve quality of compressed content. If you do not choose a filter, no filter will be applied.\\nTEMPORAL: This filter is useful for both source content that is noisy (when it has excessive digital artifacts) and source content that is clean.\\nWhen the content is noisy, the filter cleans up the source content before the encoding phase, with these two effects: First, it improves the output video quality because the content has been cleaned up. Secondly, it decreases the bandwidth because MediaLive does not waste bits on encoding noise.\\nWhen the content is reasonably clean, the\
  \ filter tends to decrease the bitrate.\"\n        }\n      ]\n    },\n    \"FixedAfd\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FixedAfd\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fixedAfd\"\n          },\n          \"description\": \"Complete this field only when afdSignaling is set to FIXED. Enter the AFD value (4 bits) to write on all frames of the video encode.\"\n        }\n      ]\n    },\n    \"FramerateDenominator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateDenominator\"\n          },\n          \"description\": \"description\\\": \\\"The framerate denominator. For example, 1001. The framerate is the numerator divided by the denominator. For example, 24000 / 1001 = 23.976 FPS.\"\n        }\n      ]\n    },\n    \"FramerateNumerator\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/__integerMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateNumerator\"\n          },\n          \"description\": \"The framerate numerator. For example, 24000. The framerate is the numerator divided by the denominator. For example, 24000 / 1001 = 23.976 FPS.\"\n        }\n      ]\n    },\n    \"GopClosedCadence\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gopClosedCadence\"\n          },\n          \"description\": \"MPEG2: default is open GOP.\"\n        }\n      ]\n    },\n    \"GopNumBFrames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max7\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gopNumBFrames\"\n          },\n          \"description\": \"Relates to the GOP structure. The number of B-frames between reference frames. If you do\
  \ not know what a B-frame is, use the default.\"\n        }\n      ]\n    },\n    \"GopSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gopSize\"\n          },\n          \"description\": \"Relates to the GOP structure. The GOP size (keyframe interval) in the units specified in gopSizeUnits. If you do not know what GOP is, use the default.\\nIf gopSizeUnits is frames, then the gopSize must be an integer and must be greater than or equal to 1.\\nIf gopSizeUnits is seconds, the gopSize must be greater than 0, but does not need to be an integer.\"\n        }\n      ]\n    },\n    \"GopSizeUnits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2GopSizeUnits\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gopSizeUnits\"\n          },\n          \"description\": \"Relates to the GOP structure. Specifies whether the gopSize\
  \ is specified in frames or seconds. If you do not plan to change the default gopSize, leave the default. If you specify SECONDS, MediaLive will internally convert the gop size to a frame count.\"\n        }\n      ]\n    },\n    \"ScanType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2ScanType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scanType\"\n          },\n          \"description\": \"Set the scan type of the output to PROGRESSIVE or INTERLACED (top field first).\"\n        }\n      ]\n    },\n    \"SubgopLength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2SubGopLength\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"subgopLength\"\n          },\n          \"description\": \"Relates to the GOP structure. If you do not know what GOP is, use the default.\\nFIXED: Set the number of B-frames in each sub-GOP to the value in gopNumBFrames.\\nDYNAMIC: Let MediaLive\
  \ optimize the number of B-frames in each sub-GOP, to improve visual quality.\"\n        }\n      ]\n    },\n    \"TimecodeInsertion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2TimecodeInsertionBehavior\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timecodeInsertion\"\n          },\n          \"description\": \"Determines how MediaLive inserts timecodes in the output video. For detailed information about setting up the input and the output for a timecode, see the section on \\\\\\\"MediaLive Features - Timecode configuration\\\\\\\" in the MediaLive User Guide.\\nDISABLED: do not include timecodes.\\nGOP_TIMECODE: Include timecode metadata in the GOP header.\"\n        }\n      ]\n    },\n    \"TimecodeBurninSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimecodeBurninSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timecodeBurninSettings\"\n    \
  \      },\n          \"description\": \"Timecode burn-in settings\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FramerateNumerator\",\n    \"FramerateDenominator\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-mpeg2-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Mpeg2Settings
---
