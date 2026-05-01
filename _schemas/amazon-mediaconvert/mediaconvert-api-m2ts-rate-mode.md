---
description: When set to CBR, inserts null packets into transport stream to fill specified bitrate. When set to VBR, the bitrate setting acts as the maximum bitrate, but the output will not be padded up to that bitrate.
layout: schema
name: M2tsRateMode
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-m2ts-rate-mode-schema.json
slug: mediaconvert-api-m2ts-rate-mode
source_filename: mediaconvert-api-m2ts-rate-mode-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-m2ts-rate-mode-schema.json\",\n  \"title\": \"M2tsRateMode\",\n  \"description\": \"When set to CBR, inserts null packets into transport stream to fill specified bitrate. When set to VBR, the bitrate setting acts as the maximum bitrate, but the output will not be padded up to that bitrate.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"VBR\",\n    \"CBR\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-m2ts-rate-mode-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: M2tsRateMode
---
