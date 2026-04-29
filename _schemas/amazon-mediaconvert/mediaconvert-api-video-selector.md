---
description: Input video selectors contain the video settings for the input. Each of your inputs can have up to one video selector.
layout: schema
name: VideoSelector
properties_list:
- description: ''
  name: AlphaBehavior
  type: object
- description: ''
  name: ColorSpace
  type: object
- description: ''
  name: ColorSpaceUsage
  type: object
- description: ''
  name: EmbeddedTimecodeOverride
  type: object
- description: ''
  name: Hdr10Metadata
  type: object
- description: ''
  name: PadVideo
  type: object
- description: ''
  name: Pid
  type: object
- description: ''
  name: ProgramNumber
  type: object
- description: ''
  name: Rotate
  type: object
- description: ''
  name: SampleRange
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-video-selector-schema.json
slug: mediaconvert-api-video-selector
source_filename: mediaconvert-api-video-selector-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-video-selector-schema.json\",\n  \"title\": \"VideoSelector\",\n  \"description\": \"Input video selectors contain the video settings for the input. Each of your inputs can have up to one video selector.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AlphaBehavior\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlphaBehavior\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"alphaBehavior\"\n          },\n          \"description\": \"Ignore this setting unless this input is a QuickTime animation with an alpha channel. Use this setting to create separate Key and Fill outputs. In each output, specify which part of the input MediaConvert uses. Leave this setting at the default value DISCARD to delete the alpha channel and preserve\
  \ the video. Set it to REMAP_TO_LUMA to delete the video and map the alpha channel to the luma channel of your outputs.\"\n        }\n      ]\n    },\n    \"ColorSpace\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ColorSpace\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"colorSpace\"\n          },\n          \"description\": \"If your input video has accurate color space metadata, or if you don't know about color space: Keep the default value, Follow. MediaConvert will automatically detect your input color space. If your input video has metadata indicating the wrong color space, or has missing metadata: Specify the accurate color space here. If your input video is HDR 10 and the SMPTE ST 2086 Mastering Display Color Volume static metadata isn't present in your video stream, or if that metadata is present but not accurate: Choose Force HDR 10. Specify correct values in the input HDR 10 metadata settings. For more information about\
  \ HDR jobs, see https://docs.aws.amazon.com/console/mediaconvert/hdr. When you specify an input color space, MediaConvert uses the following color space metadata, which includes color primaries, transfer characteristics, and matrix coefficients:\\n * HDR 10: BT.2020, PQ, BT.2020 non-constant\\n * HLG 2020: BT.2020, HLG, BT.2020 non-constant\\n * P3DCI (Theater): DCIP3, SMPTE 428M, BT.709\\n * P3D65 (SDR): Display P3, sRGB, BT.709\\n * P3D65 (HDR): Display P3, PQ, BT.709\"\n        }\n      ]\n    },\n    \"ColorSpaceUsage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ColorSpaceUsage\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"colorSpaceUsage\"\n          },\n          \"description\": \"There are two sources for color metadata, the input file and the job input settings Color space (ColorSpace) and HDR master display information settings(Hdr10Metadata). The Color space usage setting determines which takes precedence. Choose Force\
  \ (FORCE) to use color metadata from the input job settings. If you don't specify values for those settings, the service defaults to using metadata from your input. FALLBACK - Choose Fallback (FALLBACK) to use color metadata from the source when it is present. If there's no color metadata in your input file, the service defaults to using values you specify in the input settings.\"\n        }\n      ]\n    },\n    \"EmbeddedTimecodeOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmbeddedTimecodeOverride\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"embeddedTimecodeOverride\"\n          },\n          \"description\": \"Set Embedded timecode override (embeddedTimecodeOverride) to Use MDPM (USE_MDPM) when your AVCHD input contains timecode tag data in the Modified Digital Video Pack Metadata (MDPM). When you do, we recommend you also set Timecode source (inputTimecodeSource) to Embedded (EMBEDDED). Leave Embedded timecode override\
  \ blank, or set to None (NONE), when your input does not contain MDPM timecode.\"\n        }\n      ]\n    },\n    \"Hdr10Metadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Hdr10Metadata\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hdr10Metadata\"\n          },\n          \"description\": \"Use these settings to provide HDR 10 metadata that is missing or inaccurate in your input video. Appropriate values vary depending on the input video and must be provided by a color grader. The color grader generates these values during the HDR 10 mastering process. The valid range for each of these settings is 0 to 50,000. Each increment represents 0.00002 in CIE1931 color coordinate. Related settings - When you specify these values, you must also set Color space (ColorSpace) to HDR 10 (HDR10). To specify whether the the values you specify here take precedence over the values in the metadata of your input file, set Color space usage (ColorSpaceUsage).\
  \ To specify whether color metadata is included in an output, set Color metadata (ColorMetadata). For more information about MediaConvert HDR jobs, see https://docs.aws.amazon.com/console/mediaconvert/hdr.\"\n        }\n      ]\n    },\n    \"PadVideo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PadVideo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"padVideo\"\n          },\n          \"description\": \"Use this setting if your input has video and audio durations that don't align, and your output or player has strict alignment requirements. Examples: Input audio track has a delayed start. Input video track ends before audio ends. When you set Pad video (padVideo) to Black (BLACK), MediaConvert generates black video frames so that output video and audio durations match. Black video frames are added at the beginning or end, depending on your input. To keep the default behavior and not generate black video, set Pad video to Disabled\
  \ (DISABLED) or leave blank.\"\n        }\n      ]\n    },\n    \"Pid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pid\"\n          },\n          \"description\": \"Use PID (Pid) to select specific video data from an input file. Specify this value as an integer; the system automatically converts it to the hexidecimal value. For example, 257 selects PID 0x101. A PID, or packet identifier, is an identifier for a set of data in an MPEG-2 transport stream container.\"\n        }\n      ]\n    },\n    \"ProgramNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMinNegative2147483648Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"programNumber\"\n          },\n          \"description\": \"Selects a specific program from within a multi-program transport stream. Note that Quad 4K is\
  \ not currently supported.\"\n        }\n      ]\n    },\n    \"Rotate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputRotate\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"rotate\"\n          },\n          \"description\": \"Use Rotate (InputRotate) to specify how the service rotates your video. You can choose automatic rotation or specify a rotation. You can specify a clockwise rotation of 0, 90, 180, or 270 degrees. If your input video container is .mov or .mp4 and your input has rotation metadata, you can choose Automatic to have the service rotate your video according to the rotation specified in the metadata. The rotation must be within one degree of 90, 180, or 270 degrees. If the rotation metadata specifies any other rotation, the service will default to no rotation. By default, the service does no rotation, even if your input video has rotation metadata. The service doesn't pass through rotation metadata.\"\n      \
  \  }\n      ]\n    },\n    \"SampleRange\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputSampleRange\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sampleRange\"\n          },\n          \"description\": \"If the sample range metadata in your input video is accurate, or if you don't know about sample range, keep the default value, Follow (FOLLOW), for this setting. When you do, the service automatically detects your input sample range. If your input video has metadata indicating the wrong sample range, specify the accurate sample range here. When you do, MediaConvert ignores any sample range information in the input metadata. Regardless of whether MediaConvert uses the input sample range or the sample range that you specify, MediaConvert uses the sample range for transcoding and also writes it to the output metadata.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-video-selector-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: VideoSelector
---
