---
description: Optional. Ignore this setting unless Nagra support directs you to specify a value. When you don't specify a value here, the Nagra NexGuard library uses its default value.
layout: schema
name: WatermarkingStrength
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-watermarking-strength-schema.json
slug: mediaconvert-api-watermarking-strength
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-watermarking-strength-schema.json\",\n  \"title\": \"WatermarkingStrength\",\n  \"description\": \"Optional. Ignore this setting unless Nagra support directs you to specify a value. When you don't specify a value here, the Nagra NexGuard library uses its default value.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"LIGHTEST\",\n    \"LIGHTER\",\n    \"DEFAULT\",\n    \"STRONGER\",\n    \"STRONGEST\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-watermarking-strength-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: WatermarkingStrength
---
