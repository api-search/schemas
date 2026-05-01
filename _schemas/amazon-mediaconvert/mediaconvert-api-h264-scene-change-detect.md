---
description: Enable this setting to insert I-frames at scene changes that the service automatically detects. This improves video quality and is enabled by default. If this output uses QVBR, choose Transition detection (TRANSITION_DETECTION) for further video quality improvement. For more information about QVBR, see https://docs.aws.amazon.com/console/mediaconvert/cbr-vbr-qvbr.
layout: schema
name: H264SceneChangeDetect
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-h264-scene-change-detect-schema.json
slug: mediaconvert-api-h264-scene-change-detect
source_filename: mediaconvert-api-h264-scene-change-detect-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-h264-scene-change-detect-schema.json\",\n  \"title\": \"H264SceneChangeDetect\",\n  \"description\": \"Enable this setting to insert I-frames at scene changes that the service automatically detects. This improves video quality and is enabled by default. If this output uses QVBR, choose Transition detection (TRANSITION_DETECTION) for further video quality improvement. For more information about QVBR, see https://docs.aws.amazon.com/console/mediaconvert/cbr-vbr-qvbr.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"DISABLED\",\n    \"ENABLED\",\n    \"TRANSITION_DETECTION\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-h264-scene-change-detect-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: H264SceneChangeDetect
---
