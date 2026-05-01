---
description: If set to PROGRESSIVE_DOWNLOAD, the MOOV atom is relocated to the beginning of the archive as required for progressive downloading. Otherwise it is placed normally at the end.
layout: schema
name: F4vMoovPlacement
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-f4v-moov-placement-schema.json
slug: mediaconvert-api-f4v-moov-placement
source_filename: mediaconvert-api-f4v-moov-placement-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-f4v-moov-placement-schema.json\",\n  \"title\": \"F4vMoovPlacement\",\n  \"description\": \"If set to PROGRESSIVE_DOWNLOAD, the MOOV atom is relocated to the beginning of the archive as required for progressive downloading. Otherwise it is placed normally at the end.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"PROGRESSIVE_DOWNLOAD\",\n    \"NORMAL\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-f4v-moov-placement-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: F4vMoovPlacement
---
