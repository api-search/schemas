---
description: When enabled the output audio is corrected using the chosen algorithm. If disabled, the audio will be measured but not adjusted.
layout: schema
name: AudioNormalizationAlgorithmControl
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-audio-normalization-algorithm-control-schema.json
slug: mediaconvert-api-audio-normalization-algorithm-control
source_filename: mediaconvert-api-audio-normalization-algorithm-control-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-audio-normalization-algorithm-control-schema.json\",\n  \"title\": \"AudioNormalizationAlgorithmControl\",\n  \"description\": \"When enabled the output audio is corrected using the chosen algorithm. If disabled, the audio will be measured but not adjusted.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"CORRECT_AUDIO\",\n    \"MEASURE_ONLY\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-audio-normalization-algorithm-control-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: AudioNormalizationAlgorithmControl
---
