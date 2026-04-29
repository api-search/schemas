---
description: Specify whether the Text spacing (TeletextSpacing) in your captions is set by the captions grid, or varies depending on letter width. Choose fixed grid (FIXED_GRID) to conform to the spacing specified in the captions file more accurately. Choose proportional (PROPORTIONAL) to make the text easier to read for closed captions. Within your job settings, all of your DVB-Sub settings must be identical.
layout: schema
name: DvbSubtitleTeletextSpacing
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-dvb-subtitle-teletext-spacing-schema.json
slug: mediaconvert-api-dvb-subtitle-teletext-spacing
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dvb-subtitle-teletext-spacing-schema.json\",\n  \"title\": \"DvbSubtitleTeletextSpacing\",\n  \"description\": \"Specify whether the Text spacing (TeletextSpacing) in your captions is set by the captions grid, or varies depending on letter width. Choose fixed grid (FIXED_GRID) to conform to the spacing specified in the captions file more accurately. Choose proportional (PROPORTIONAL) to make the text easier to read for closed captions. Within your job settings, all of your DVB-Sub settings must be identical.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"FIXED_GRID\",\n    \"PROPORTIONAL\",\n    \"AUTO\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dvb-subtitle-teletext-spacing-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DvbSubtitleTeletextSpacing
---
