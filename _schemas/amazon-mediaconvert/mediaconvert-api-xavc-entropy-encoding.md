---
description: Optional. Choose a specific entropy encoding mode only when you want to override XAVC recommendations. If you choose the value auto, MediaConvert uses the mode that the XAVC file format specifies given this output's operating point.
layout: schema
name: XavcEntropyEncoding
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-xavc-entropy-encoding-schema.json
slug: mediaconvert-api-xavc-entropy-encoding
source_filename: mediaconvert-api-xavc-entropy-encoding-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-xavc-entropy-encoding-schema.json\",\n  \"title\": \"XavcEntropyEncoding\",\n  \"description\": \"Optional. Choose a specific entropy encoding mode only when you want to override XAVC recommendations. If you choose the value auto, MediaConvert uses the mode that the XAVC file format specifies given this output's operating point.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"AUTO\",\n    \"CABAC\",\n    \"CAVLC\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-xavc-entropy-encoding-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: XavcEntropyEncoding
---
