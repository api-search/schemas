---
description: To transcode only portions of your input, include one input clip for each part of your input that you want in your output. All input clips that you specify will be included in every output of the job. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/assembling-multiple-inputs-and-input-clips.html.
layout: schema
name: InputClipping
properties_list:
- description: ''
  name: EndTimecode
  type: object
- description: ''
  name: StartTimecode
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-input-clipping-schema.json
slug: mediaconvert-api-input-clipping
source_filename: mediaconvert-api-input-clipping-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-input-clipping-schema.json\",\n  \"title\": \"InputClipping\",\n  \"description\": \"To transcode only portions of your input, include one input clip for each part of your input that you want in your output. All input clips that you specify will be included in every output of the job. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/assembling-multiple-inputs-and-input-clips.html.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndTimecode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPattern010920405090509092\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"endTimecode\"\n          },\n          \"description\": \"Set End timecode (EndTimecode) to the end of the portion of the input\
  \ you are clipping. The frame corresponding to the End timecode value is included in the clip. Start timecode or End timecode may be left blank, but not both. Use the format HH:MM:SS:FF or HH:MM:SS;FF, where HH is the hour, MM is the minute, SS is the second, and FF is the frame number. When choosing this value, take into account your setting for timecode source under input settings (InputTimecodeSource). For example, if you have embedded timecodes that start at 01:00:00:00 and you want your clip to end six minutes into the video, use 01:06:00:00.\"\n        }\n      ]\n    },\n    \"StartTimecode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPattern010920405090509092\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"startTimecode\"\n          },\n          \"description\": \"Set Start timecode (StartTimecode) to the beginning of the portion of the input you are clipping. The frame corresponding to the Start timecode value\
  \ is included in the clip. Start timecode or End timecode may be left blank, but not both. Use the format HH:MM:SS:FF or HH:MM:SS;FF, where HH is the hour, MM is the minute, SS is the second, and FF is the frame number. When choosing this value, take into account your setting for Input timecode source. For example, if you have embedded timecodes that start at 01:00:00:00 and you want your clip to begin five minutes into the video, use 01:05:00:00.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-input-clipping-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: InputClipping
---
