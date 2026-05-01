---
description: Input resolution based on lines of vertical resolution in the input; SD is less than 720 lines, HD is 720 to 1080 lines, UHD is greater than 1080 lines
layout: schema
name: InputResolution
properties_list: []
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-input-resolution-schema.json
slug: medialive-api-input-resolution
source_filename: medialive-api-input-resolution-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-resolution-schema.json\",\n  \"title\": \"InputResolution\",\n  \"description\": \"Input resolution based on lines of vertical resolution in the input; SD is less than 720 lines, HD is 720 to 1080 lines, UHD is greater than 1080 lines\\n\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"SD\",\n    \"HD\",\n    \"UHD\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-resolution-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: InputResolution
---
