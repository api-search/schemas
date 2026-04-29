---
description: Only applies when you set Deinterlacer (DeinterlaceMode) to Deinterlace (DEINTERLACE) or Adaptive (ADAPTIVE). Motion adaptive interpolate (INTERPOLATE) produces sharper pictures, while blend (BLEND) produces smoother motion. Use (INTERPOLATE_TICKER) OR (BLEND_TICKER) if your source file includes a ticker, such as a scrolling headline at the bottom of the frame.
layout: schema
name: DeinterlaceAlgorithm
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-deinterlace-algorithm-schema.json
slug: mediaconvert-api-deinterlace-algorithm
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-deinterlace-algorithm-schema.json\",\n  \"title\": \"DeinterlaceAlgorithm\",\n  \"description\": \"Only applies when you set Deinterlacer (DeinterlaceMode) to Deinterlace (DEINTERLACE) or Adaptive (ADAPTIVE). Motion adaptive interpolate (INTERPOLATE) produces sharper pictures, while blend (BLEND) produces smoother motion. Use (INTERPOLATE_TICKER) OR (BLEND_TICKER) if your source file includes a ticker, such as a scrolling headline at the bottom of the frame.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"INTERPOLATE\",\n    \"INTERPOLATE_TICKER\",\n    \"BLEND\",\n    \"BLEND_TICKER\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-deinterlace-algorithm-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DeinterlaceAlgorithm
---
