---
description: The service defaults to using RIFF for WAV outputs. If your output audio is likely to exceed 4 GB in file size, or if you otherwise need the extended support of the RF64 format, set your output WAV file format to RF64.
layout: schema
name: WavFormat
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-wav-format-schema.json
slug: mediaconvert-api-wav-format
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-wav-format-schema.json\",\n  \"title\": \"WavFormat\",\n  \"description\": \"The service defaults to using RIFF for WAV outputs. If your output audio is likely to exceed 4 GB in file size, or if you otherwise need the extended support of the RF64 format, set your output WAV file format to RF64.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"RIFF\",\n    \"RF64\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-wav-format-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: WavFormat
---
