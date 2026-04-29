---
description: Use Deinterlacer (DeinterlaceMode) to choose how the service will do deinterlacing. Default is Deinterlace. - Deinterlace converts interlaced to progressive. - Inverse telecine converts Hard Telecine 29.97i to progressive 23.976p. - Adaptive auto-detects and converts to progressive.
layout: schema
name: DeinterlacerMode
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-deinterlacer-mode-schema.json
slug: mediaconvert-api-deinterlacer-mode
source_filename: mediaconvert-api-deinterlacer-mode-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-deinterlacer-mode-schema.json\",\n  \"title\": \"DeinterlacerMode\",\n  \"description\": \"Use Deinterlacer (DeinterlaceMode) to choose how the service will do deinterlacing. Default is Deinterlace. - Deinterlace converts interlaced to progressive. - Inverse telecine converts Hard Telecine 29.97i to progressive 23.976p. - Adaptive auto-detects and converts to progressive.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"DEINTERLACE\",\n    \"INVERSE_TELECINE\",\n    \"ADAPTIVE\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-deinterlacer-mode-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DeinterlacerMode
---
