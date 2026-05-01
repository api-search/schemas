---
description: Enable Deblock (InputDeblockFilter) to produce smoother motion in the output. Default is disabled. Only manually controllable for MPEG2 and uncompressed video inputs.
layout: schema
name: InputDeblockFilter
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-input-deblock-filter-schema.json
slug: mediaconvert-api-input-deblock-filter
source_filename: mediaconvert-api-input-deblock-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-input-deblock-filter-schema.json\",\n  \"title\": \"InputDeblockFilter\",\n  \"description\": \"Enable Deblock (InputDeblockFilter) to produce smoother motion in the output. Default is disabled. Only manually controllable for MPEG2 and uncompressed video inputs.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"ENABLED\",\n    \"DISABLED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-input-deblock-filter-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: InputDeblockFilter
---
