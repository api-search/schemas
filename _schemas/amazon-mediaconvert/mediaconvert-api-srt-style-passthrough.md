---
description: Set Style passthrough (StylePassthrough) to ENABLED to use the available style, color, and position information from your input captions. MediaConvert uses default settings for any missing style and position information in your input captions. Set Style passthrough to DISABLED, or leave blank, to ignore the style and position information from your input captions and use simplified output captions.
layout: schema
name: SrtStylePassthrough
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-srt-style-passthrough-schema.json
slug: mediaconvert-api-srt-style-passthrough
source_filename: mediaconvert-api-srt-style-passthrough-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-srt-style-passthrough-schema.json\",\n  \"title\": \"SrtStylePassthrough\",\n  \"description\": \"Set Style passthrough (StylePassthrough) to ENABLED to use the available style, color, and position information from your input captions. MediaConvert uses default settings for any missing style and position information in your input captions. Set Style passthrough to DISABLED, or leave blank, to ignore the style and position information from your input captions and use simplified output captions.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"ENABLED\",\n    \"DISABLED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-srt-style-passthrough-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: SrtStylePassthrough
---
