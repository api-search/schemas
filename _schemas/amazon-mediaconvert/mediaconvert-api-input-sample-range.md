---
description: If the sample range metadata in your input video is accurate, or if you don't know about sample range, keep the default value, Follow (FOLLOW), for this setting. When you do, the service automatically detects your input sample range. If your input video has metadata indicating the wrong sample range, specify the accurate sample range here. When you do, MediaConvert ignores any sample range information in the input metadata. Regardless of whether MediaConvert uses the input sample range or the sample range that you specify, MediaConvert uses the sample range for transcoding and also writes it to the output metadata.
layout: schema
name: InputSampleRange
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-input-sample-range-schema.json
slug: mediaconvert-api-input-sample-range
source_filename: mediaconvert-api-input-sample-range-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-input-sample-range-schema.json\",\n  \"title\": \"InputSampleRange\",\n  \"description\": \"If the sample range metadata in your input video is accurate, or if you don't know about sample range, keep the default value, Follow (FOLLOW), for this setting. When you do, the service automatically detects your input sample range. If your input video has metadata indicating the wrong sample range, specify the accurate sample range here. When you do, MediaConvert ignores any sample range information in the input metadata. Regardless of whether MediaConvert uses the input sample range or the sample range that you specify, MediaConvert uses the sample range for transcoding and also writes it to the output metadata.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"FOLLOW\",\n    \"FULL_RANGE\"\
  ,\n    \"LIMITED_RANGE\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-input-sample-range-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: InputSampleRange
---
