---
description: Choose Adaptive to improve subjective video quality for high-motion content. This will cause the service to use fewer B-frames (which infer information based on other frames) for high-motion portions of the video and more B-frames for low-motion portions. The maximum number of B-frames is limited by the value you provide for the setting B frames between reference frames (numberBFramesBetweenReferenceFrames).
layout: schema
name: H265DynamicSubGop
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-h265-dynamic-sub-gop-schema.json
slug: mediaconvert-api-h265-dynamic-sub-gop
source_filename: mediaconvert-api-h265-dynamic-sub-gop-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-h265-dynamic-sub-gop-schema.json\",\n  \"title\": \"H265DynamicSubGop\",\n  \"description\": \"Choose Adaptive to improve subjective video quality for high-motion content. This will cause the service to use fewer B-frames (which infer information based on other frames) for high-motion portions of the video and more B-frames for low-motion portions. The maximum number of B-frames is limited by the value you provide for the setting B frames between reference frames (numberBFramesBetweenReferenceFrames).\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"ADAPTIVE\",\n    \"STATIC\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-h265-dynamic-sub-gop-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: H265DynamicSubGop
---
