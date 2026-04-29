---
description: 'Keep the default value, Auto (AUTO), for this setting to have MediaConvert automatically apply the best types of quantization for your video content. When you want to apply your quantization settings manually, you must set Adaptive quantization (adaptiveQuantization) to a value other than Auto (AUTO). Use this setting to specify the strength of any adaptive quantization filters that you enable. If you don''t want MediaConvert to do any adaptive quantization in this transcode, set Adaptive quantization to Off (OFF). Related settings: The value that you choose here applies to the following settings: Flicker adaptive quantization (flickerAdaptiveQuantization), Spatial adaptive quantization (spatialAdaptiveQuantization), and Temporal adaptive quantization (temporalAdaptiveQuantization).'
layout: schema
name: XavcAdaptiveQuantization
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-xavc-adaptive-quantization-schema.json
slug: mediaconvert-api-xavc-adaptive-quantization
source_filename: mediaconvert-api-xavc-adaptive-quantization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-xavc-adaptive-quantization-schema.json\",\n  \"title\": \"XavcAdaptiveQuantization\",\n  \"description\": \"Keep the default value, Auto (AUTO), for this setting to have MediaConvert automatically apply the best types of quantization for your video content. When you want to apply your quantization settings manually, you must set Adaptive quantization (adaptiveQuantization) to a value other than Auto (AUTO). Use this setting to specify the strength of any adaptive quantization filters that you enable. If you don't want MediaConvert to do any adaptive quantization in this transcode, set Adaptive quantization to Off (OFF). Related settings: The value that you choose here applies to the following settings: Flicker adaptive quantization (flickerAdaptiveQuantization), Spatial adaptive quantization\
  \ (spatialAdaptiveQuantization), and Temporal adaptive quantization (temporalAdaptiveQuantization).\",\n  \"type\": \"string\",\n  \"enum\": [\n    false,\n    \"AUTO\",\n    \"LOW\",\n    \"MEDIUM\",\n    \"HIGH\",\n    \"HIGHER\",\n    \"MAX\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-xavc-adaptive-quantization-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: XavcAdaptiveQuantization
---
