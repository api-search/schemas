---
description: When set to VIDEO_AND_FIXED_INTERVALS, audio EBP markers will be added to partitions 3 and 4. The interval between these additional markers will be fixed, and will be slightly shorter than the video EBP marker interval. When set to VIDEO_INTERVAL, these additional markers will not be inserted. Only applicable when EBP segmentation markers are is selected (segmentationMarkers is EBP or EBP_LEGACY).
layout: schema
name: M2tsEbpAudioInterval
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-m2ts-ebp-audio-interval-schema.json
slug: mediaconvert-api-m2ts-ebp-audio-interval
source_filename: mediaconvert-api-m2ts-ebp-audio-interval-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-m2ts-ebp-audio-interval-schema.json\",\n  \"title\": \"M2tsEbpAudioInterval\",\n  \"description\": \"When set to VIDEO_AND_FIXED_INTERVALS, audio EBP markers will be added to partitions 3 and 4. The interval between these additional markers will be fixed, and will be slightly shorter than the video EBP marker interval. When set to VIDEO_INTERVAL, these additional markers will not be inserted. Only applicable when EBP segmentation markers are is selected (segmentationMarkers is EBP or EBP_LEGACY).\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"VIDEO_AND_FIXED_INTERVALS\",\n    \"VIDEO_INTERVAL\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-m2ts-ebp-audio-interval-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: M2tsEbpAudioInterval
---
