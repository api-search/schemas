---
description: Specify the font that you want the service to use for your burn in captions when your input captions specify a font that MediaConvert doesn't support. When you set Fallback font (FallbackFont) to best match (BEST_MATCH), or leave blank, MediaConvert uses a supported font that most closely matches the font that your input captions specify. When there are multiple unsupported fonts in your input captions, MediaConvert matches each font with the supported font that matches best. When you explicitly choose a replacement font, MediaConvert uses that font to replace all unsupported fonts from your input.
layout: schema
name: DvbSubSubtitleFallbackFont
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-dvb-sub-subtitle-fallback-font-schema.json
slug: mediaconvert-api-dvb-sub-subtitle-fallback-font
source_filename: mediaconvert-api-dvb-sub-subtitle-fallback-font-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dvb-sub-subtitle-fallback-font-schema.json\",\n  \"title\": \"DvbSubSubtitleFallbackFont\",\n  \"description\": \"Specify the font that you want the service to use for your burn in captions when your input captions specify a font that MediaConvert doesn't support. When you set Fallback font (FallbackFont) to best match (BEST_MATCH), or leave blank, MediaConvert uses a supported font that most closely matches the font that your input captions specify. When there are multiple unsupported fonts in your input captions, MediaConvert matches each font with the supported font that matches best. When you explicitly choose a replacement font, MediaConvert uses that font to replace all unsupported fonts from your input.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"BEST_MATCH\",\n    \"\
  MONOSPACED_SANSSERIF\",\n    \"MONOSPACED_SERIF\",\n    \"PROPORTIONAL_SANSSERIF\",\n    \"PROPORTIONAL_SERIF\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dvb-sub-subtitle-fallback-font-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: DvbSubSubtitleFallbackFont
---
