---
description: If your input captions are SCC, SMI, SRT, STL, TTML, WebVTT, or IMSC 1.1 in an xml file, specify the URI of the input caption source file. If your caption source is IMSC in an IMF package, use TrackSourceSettings instead of FileSoureSettings.
layout: schema
name: FileSourceSettings
properties_list:
- description: ''
  name: Convert608To708
  type: object
- description: ''
  name: Framerate
  type: object
- description: ''
  name: SourceFile
  type: object
- description: ''
  name: TimeDelta
  type: object
- description: ''
  name: TimeDeltaUnits
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-file-source-settings-schema.json
slug: mediaconvert-api-file-source-settings
source_filename: mediaconvert-api-file-source-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-file-source-settings-schema.json\",\n  \"title\": \"FileSourceSettings\",\n  \"description\": \"If your input captions are SCC, SMI, SRT, STL, TTML, WebVTT, or IMSC 1.1 in an xml file, specify the URI of the input caption source file. If your caption source is IMSC in an IMF package, use TrackSourceSettings instead of FileSoureSettings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Convert608To708\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileSourceConvert608To708\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"convert608To708\"\n          },\n          \"description\": \"Specify whether this set of input captions appears in your outputs in both 608 and 708 format. If you choose Upconvert (UPCONVERT), MediaConvert\
  \ includes the captions data in two ways: it passes the 608 data through using the 608 compatibility bytes fields of the 708 wrapper, and it also translates the 608 data into 708.\"\n        }\n      ]\n    },\n    \"Framerate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CaptionSourceFramerate\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerate\"\n          },\n          \"description\": \"Ignore this setting unless your input captions format is SCC. To have the service compensate for differing frame rates between your input captions and input video, specify the frame rate of the captions file. Specify this value as a fraction. When you work directly in your JSON job specification, use the settings framerateNumerator and framerateDenominator. For example, you might specify 24 / 1 for 24 fps, 25 / 1 for 25 fps, 24000 / 1001 for 23.976 fps, or 30000 / 1001 for 29.97 fps.\"\n        }\n      ]\n    },\n    \"SourceFile\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin14PatternS3SccSCCTtmlTTMLDfxpDFXPStlSTLSrtSRTXmlXMLSmiSMIVttVTTWebvttWEBVTTHttpsSccSCCTtmlTTMLDfxpDFXPStlSTLSrtSRTXmlXMLSmiSMIVttVTTWebvttWEBVTT\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sourceFile\"\n          },\n          \"description\": \"External caption file used for loading captions. Accepted file extensions are 'scc', 'ttml', 'dfxp', 'stl', 'srt', 'xml', 'smi', 'webvtt', and 'vtt'.\"\n        }\n      ]\n    },\n    \"TimeDelta\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMinNegative2147483648Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timeDelta\"\n          },\n          \"description\": \"Optional. Use this setting when you need to adjust the sync between your sidecar captions and your video. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/time-delta-use-cases.html.\
  \ Enter a positive or negative number to modify the times in the captions file. For example, type 15 to add 15 seconds to all the times in the captions file. Type -5 to subtract 5 seconds from the times in the captions file. You can optionally specify your time delta in milliseconds instead of seconds. When you do so, set the related setting, Time delta units (TimeDeltaUnits) to Milliseconds (MILLISECONDS). Note that, when you specify a time delta for timecode-based caption sources, such as SCC and STL, and your time delta isn't a multiple of the input frame rate, MediaConvert snaps the captions to the nearest frame. For example, when your input video frame rate is 25 fps and you specify 1010ms for time delta, MediaConvert delays your captions by 1000 ms.\"\n        }\n      ]\n    },\n    \"TimeDeltaUnits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileSourceTimeDeltaUnits\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timeDeltaUnits\"\
  \n          },\n          \"description\": \"When you use the setting Time delta (TimeDelta) to adjust the sync between your sidecar captions and your video, use this setting to specify the units for the delta that you specify. When you don't specify a value for Time delta units (TimeDeltaUnits), MediaConvert uses seconds by default.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-file-source-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: FileSourceSettings
---
