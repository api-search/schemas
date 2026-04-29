---
description: When you set Adaptive Quantization (H265AdaptiveQuantization) to Auto (AUTO), or leave blank, MediaConvert automatically applies quantization to improve the video quality of your output. Set Adaptive Quantization to Low (LOW), Medium (MEDIUM), High (HIGH), Higher (HIGHER), or Max (MAX) to manually control the strength of the quantization filter. When you do, you can specify a value for Spatial Adaptive Quantization (H265SpatialAdaptiveQuantization), Temporal Adaptive Quantization (H265TemporalAdaptiveQuantization), and Flicker Adaptive Quantization (H265FlickerAdaptiveQuantization), to further control the quantization filter. Set Adaptive Quantization to Off (OFF) to apply no quantization to your output.
layout: schema
name: H265AdaptiveQuantization
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-h265-adaptive-quantization-schema.json
slug: mediaconvert-api-h265-adaptive-quantization
source_filename: mediaconvert-api-h265-adaptive-quantization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-h265-adaptive-quantization-schema.json\",\n  \"title\": \"H265AdaptiveQuantization\",\n  \"description\": \"When you set Adaptive Quantization (H265AdaptiveQuantization) to Auto (AUTO), or leave blank, MediaConvert automatically applies quantization to improve the video quality of your output. Set Adaptive Quantization to Low (LOW), Medium (MEDIUM), High (HIGH), Higher (HIGHER), or Max (MAX) to manually control the strength of the quantization filter. When you do, you can specify a value for Spatial Adaptive Quantization (H265SpatialAdaptiveQuantization), Temporal Adaptive Quantization (H265TemporalAdaptiveQuantization), and Flicker Adaptive Quantization (H265FlickerAdaptiveQuantization), to further control the quantization filter. Set Adaptive Quantization to Off (OFF) to apply no\
  \ quantization to your output.\",\n  \"type\": \"string\",\n  \"enum\": [\n    false,\n    \"LOW\",\n    \"MEDIUM\",\n    \"HIGH\",\n    \"HIGHER\",\n    \"MAX\",\n    \"AUTO\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-h265-adaptive-quantization-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: H265AdaptiveQuantization
---
