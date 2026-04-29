---
description: Specify whether the text spacing (TeletextSpacing) in your captions is set by the captions grid, or varies depending on letter width. Choose fixed grid (FIXED_GRID) to conform to the spacing specified in the captions file more accurately. Choose proportional (PROPORTIONAL) to make the text easier to read for closed captions.
layout: schema
name: BurninSubtitleTeletextSpacing
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-burnin-subtitle-teletext-spacing-schema.json
slug: mediaconvert-api-burnin-subtitle-teletext-spacing
source_filename: mediaconvert-api-burnin-subtitle-teletext-spacing-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-burnin-subtitle-teletext-spacing-schema.json\",\n  \"title\": \"BurninSubtitleTeletextSpacing\",\n  \"description\": \"Specify whether the text spacing (TeletextSpacing) in your captions is set by the captions grid, or varies depending on letter width. Choose fixed grid (FIXED_GRID) to conform to the spacing specified in the captions file more accurately. Choose proportional (PROPORTIONAL) to make the text easier to read for closed captions.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"FIXED_GRID\",\n    \"PROPORTIONAL\",\n    \"AUTO\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-burnin-subtitle-teletext-spacing-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: BurninSubtitleTeletextSpacing
---
