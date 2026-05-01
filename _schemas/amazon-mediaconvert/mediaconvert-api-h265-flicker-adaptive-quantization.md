---
description: 'Enable this setting to have the encoder reduce I-frame pop. I-frame pop appears as a visual flicker that can arise when the encoder saves bits by copying some macroblocks many times from frame to frame, and then refreshes them at the I-frame. When you enable this setting, the encoder updates these macroblocks slightly more often to smooth out the flicker. This setting is disabled by default. Related setting: In addition to enabling this setting, you must also set adaptiveQuantization to a value other than Off (OFF).'
layout: schema
name: H265FlickerAdaptiveQuantization
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-h265-flicker-adaptive-quantization-schema.json
slug: mediaconvert-api-h265-flicker-adaptive-quantization
source_filename: mediaconvert-api-h265-flicker-adaptive-quantization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-h265-flicker-adaptive-quantization-schema.json\",\n  \"title\": \"H265FlickerAdaptiveQuantization\",\n  \"description\": \"Enable this setting to have the encoder reduce I-frame pop. I-frame pop appears as a visual flicker that can arise when the encoder saves bits by copying some macroblocks many times from frame to frame, and then refreshes them at the I-frame. When you enable this setting, the encoder updates these macroblocks slightly more often to smooth out the flicker. This setting is disabled by default. Related setting: In addition to enabling this setting, you must also set adaptiveQuantization to a value other than Off (OFF).\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"DISABLED\",\n    \"ENABLED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-h265-flicker-adaptive-quantization-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: H265FlickerAdaptiveQuantization
---
