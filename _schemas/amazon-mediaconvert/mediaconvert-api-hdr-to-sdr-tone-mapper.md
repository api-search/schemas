---
description: 'Specify how MediaConvert maps brightness and colors from your HDR input to your SDR output. The mode that you select represents a creative choice, with different tradeoffs in the details and tones of your output. To maintain details in bright or saturated areas of your output: Choose Preserve details. For some sources, your SDR output may look less bright and less saturated when compared to your HDR source. MediaConvert automatically applies this mode for HLG sources, regardless of your choice. For a bright and saturated output: Choose Vibrant. We recommend that you choose this mode when any of your source content is HDR10, and for the best results when it is mastered for 1000 nits. You may notice loss of details in bright or saturated areas of your output. HDR to SDR tone mapping has no effect when your input is SDR.'
layout: schema
name: HDRToSDRToneMapper
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-hdr-to-sdr-tone-mapper-schema.json
slug: mediaconvert-api-hdr-to-sdr-tone-mapper
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hdr-to-sdr-tone-mapper-schema.json\",\n  \"title\": \"HDRToSDRToneMapper\",\n  \"description\": \"Specify how MediaConvert maps brightness and colors from your HDR input to your SDR output. The mode that you select represents a creative choice, with different tradeoffs in the details and tones of your output. To maintain details in bright or saturated areas of your output: Choose Preserve details. For some sources, your SDR output may look less bright and less saturated when compared to your HDR source. MediaConvert automatically applies this mode for HLG sources, regardless of your choice. For a bright and saturated output: Choose Vibrant. We recommend that you choose this mode when any of your source content is HDR10, and for the best results when it is mastered for 1000 nits. You\
  \ may notice loss of details in bright or saturated areas of your output. HDR to SDR tone mapping has no effect when your input is SDR.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"PRESERVE_DETAILS\",\n    \"VIBRANT\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hdr-to-sdr-tone-mapper-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: HDRToSDRToneMapper
---
