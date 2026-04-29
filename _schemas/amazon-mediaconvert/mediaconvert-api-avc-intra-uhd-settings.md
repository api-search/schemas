---
description: Optional when you set AVC-Intra class (avcIntraClass) to Class 4K/2K (CLASS_4K_2K). When you set AVC-Intra class to a different value, this object isn't allowed.
layout: schema
name: AvcIntraUhdSettings
properties_list:
- description: ''
  name: QualityTuningLevel
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-avc-intra-uhd-settings-schema.json
slug: mediaconvert-api-avc-intra-uhd-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-avc-intra-uhd-settings-schema.json\",\n  \"title\": \"AvcIntraUhdSettings\",\n  \"description\": \"Optional when you set AVC-Intra class (avcIntraClass) to Class 4K/2K (CLASS_4K_2K). When you set AVC-Intra class to a different value, this object isn't allowed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"QualityTuningLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AvcIntraUhdQualityTuningLevel\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"qualityTuningLevel\"\n          },\n          \"description\": \"Optional. Use Quality tuning level (qualityTuningLevel) to choose how many transcoding passes MediaConvert does with your video. When you choose Multi-pass (MULTI_PASS), your video quality is better and your output\
  \ bitrate is more accurate. That is, the actual bitrate of your output is closer to the target bitrate defined in the specification. When you choose Single-pass (SINGLE_PASS), your encoding time is faster. The default behavior is Single-pass (SINGLE_PASS).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-avc-intra-uhd-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AvcIntraUhdSettings
---
