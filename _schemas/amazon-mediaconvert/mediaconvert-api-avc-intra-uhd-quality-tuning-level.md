---
description: Optional. Use Quality tuning level (qualityTuningLevel) to choose how many transcoding passes MediaConvert does with your video. When you choose Multi-pass (MULTI_PASS), your video quality is better and your output bitrate is more accurate. That is, the actual bitrate of your output is closer to the target bitrate defined in the specification. When you choose Single-pass (SINGLE_PASS), your encoding time is faster. The default behavior is Single-pass (SINGLE_PASS).
layout: schema
name: AvcIntraUhdQualityTuningLevel
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-avc-intra-uhd-quality-tuning-level-schema.json
slug: mediaconvert-api-avc-intra-uhd-quality-tuning-level
source_filename: mediaconvert-api-avc-intra-uhd-quality-tuning-level-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-avc-intra-uhd-quality-tuning-level-schema.json\",\n  \"title\": \"AvcIntraUhdQualityTuningLevel\",\n  \"description\": \"Optional. Use Quality tuning level (qualityTuningLevel) to choose how many transcoding passes MediaConvert does with your video. When you choose Multi-pass (MULTI_PASS), your video quality is better and your output bitrate is more accurate. That is, the actual bitrate of your output is closer to the target bitrate defined in the specification. When you choose Single-pass (SINGLE_PASS), your encoding time is faster. The default behavior is Single-pass (SINGLE_PASS).\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"SINGLE_PASS\",\n    \"MULTI_PASS\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-avc-intra-uhd-quality-tuning-level-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AvcIntraUhdQualityTuningLevel
---
