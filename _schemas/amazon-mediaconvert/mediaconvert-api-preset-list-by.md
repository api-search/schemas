---
description: Optional. When you request a list of presets, you can choose to list them alphabetically by NAME or chronologically by CREATION_DATE. If you don't specify, the service will list them by name.
layout: schema
name: PresetListBy
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-preset-list-by-schema.json
slug: mediaconvert-api-preset-list-by
source_filename: mediaconvert-api-preset-list-by-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-preset-list-by-schema.json\",\n  \"title\": \"PresetListBy\",\n  \"description\": \"Optional. When you request a list of presets, you can choose to list them alphabetically by NAME or chronologically by CREATION_DATE. If you don't specify, the service will list them by name.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"NAME\",\n    \"CREATION_DATE\",\n    \"SYSTEM\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-preset-list-by-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: PresetListBy
---
