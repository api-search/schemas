---
description: These settings control how the service handles timecodes throughout the job. These settings don't affect input clipping.
layout: schema
name: TimecodeConfig
properties_list:
- description: ''
  name: Anchor
  type: object
- description: ''
  name: Source
  type: object
- description: ''
  name: Start
  type: object
- description: ''
  name: TimestampOffset
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-timecode-config-schema.json
slug: mediaconvert-api-timecode-config
source_filename: mediaconvert-api-timecode-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-timecode-config-schema.json\",\n  \"title\": \"TimecodeConfig\",\n  \"description\": \"These settings control how the service handles timecodes throughout the job. These settings don't affect input clipping.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Anchor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPattern010920405090509092\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"anchor\"\n          },\n          \"description\": \"If you use an editing platform that relies on an anchor timecode, use Anchor Timecode (Anchor) to specify a timecode that will match the input video frame to the output video frame. Use 24-hour format with frame number, (HH:MM:SS:FF) or (HH:MM:SS;FF). This setting ignores frame rate\
  \ conversion. System behavior for Anchor Timecode varies depending on your setting for Source (TimecodeSource). * If Source (TimecodeSource) is set to Specified Start (SPECIFIEDSTART), the first input frame is the specified value in Start Timecode (Start). Anchor Timecode (Anchor) and Start Timecode (Start) are used calculate output timecode. * If Source (TimecodeSource) is set to Start at 0 (ZEROBASED) the first frame is 00:00:00:00. * If Source (TimecodeSource) is set to Embedded (EMBEDDED), the first frame is the timecode value on the first input frame of the input.\"\n        }\n      ]\n    },\n    \"Source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimecodeSource\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"source\"\n          },\n          \"description\": \"Use Source (TimecodeSource) to set how timecodes are handled within this job. To make sure that your video, audio, captions, and markers are synchronized and that\
  \ time-based features, such as image inserter, work correctly, choose the Timecode source option that matches your assets. All timecodes are in a 24-hour format with frame number (HH:MM:SS:FF). * Embedded (EMBEDDED) - Use the timecode that is in the input video. If no embedded timecode is in the source, the service will use Start at 0 (ZEROBASED) instead. * Start at 0 (ZEROBASED) - Set the timecode of the initial frame to 00:00:00:00. * Specified Start (SPECIFIEDSTART) - Set the timecode of the initial frame to a value other than zero. You use Start timecode (Start) to provide this value.\"\n        }\n      ]\n    },\n    \"Start\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPattern010920405090509092\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"start\"\n          },\n          \"description\": \"Only use when you set Source (TimecodeSource) to Specified start (SPECIFIEDSTART). Use Start timecode (Start) to specify the\
  \ timecode for the initial frame. Use 24-hour format with frame number, (HH:MM:SS:FF) or (HH:MM:SS;FF).\"\n        }\n      ]\n    },\n    \"TimestampOffset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPattern0940191020191209301\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timestampOffset\"\n          },\n          \"description\": \"Only applies to outputs that support program-date-time stamp. Use Timestamp offset (TimestampOffset) to overwrite the timecode date without affecting the time and frame number. Provide the new date as a string in the format \\\"yyyy-mm-dd\\\". To use Time stamp offset, you must also enable Insert program-date-time (InsertProgramDateTime) in the output settings. For example, if the date part of your timecodes is 2002-1-25 and you want to change it to one year later, set Timestamp offset (TimestampOffset) to 2003-1-25.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-timecode-config-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: TimecodeConfig
---
