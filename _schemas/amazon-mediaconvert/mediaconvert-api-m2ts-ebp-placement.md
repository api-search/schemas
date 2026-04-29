---
description: Selects which PIDs to place EBP markers on. They can either be placed only on the video PID, or on both the video PID and all audio PIDs. Only applicable when EBP segmentation markers are is selected (segmentationMarkers is EBP or EBP_LEGACY).
layout: schema
name: M2tsEbpPlacement
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-m2ts-ebp-placement-schema.json
slug: mediaconvert-api-m2ts-ebp-placement
source_filename: mediaconvert-api-m2ts-ebp-placement-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-m2ts-ebp-placement-schema.json\",\n  \"title\": \"M2tsEbpPlacement\",\n  \"description\": \"Selects which PIDs to place EBP markers on. They can either be placed only on the video PID, or on both the video PID and all audio PIDs. Only applicable when EBP segmentation markers are is selected (segmentationMarkers is EBP or EBP_LEGACY).\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"VIDEO_AND_AUDIO_PIDS\",\n    \"VIDEO_PID\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-m2ts-ebp-placement-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: M2tsEbpPlacement
---
