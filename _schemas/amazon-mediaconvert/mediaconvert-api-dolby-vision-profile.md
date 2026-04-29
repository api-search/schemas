---
description: Required when you enable Dolby Vision. Use Profile 5 to include frame-interleaved Dolby Vision metadata in your output. Your input must include Dolby Vision metadata or an HDR10 YUV color space. Use Profile 8.1 to include frame-interleaved Dolby Vision metadata and HDR10 metadata in your output. Your input must include Dolby Vision metadata.
layout: schema
name: DolbyVisionProfile
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-dolby-vision-profile-schema.json
slug: mediaconvert-api-dolby-vision-profile
source_filename: mediaconvert-api-dolby-vision-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dolby-vision-profile-schema.json\",\n  \"title\": \"DolbyVisionProfile\",\n  \"description\": \"Required when you enable Dolby Vision. Use Profile 5 to include frame-interleaved Dolby Vision metadata in your output. Your input must include Dolby Vision metadata or an HDR10 YUV color space. Use Profile 8.1 to include frame-interleaved Dolby Vision metadata and HDR10 metadata in your output. Your input must include Dolby Vision metadata.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"PROFILE_5\",\n    \"PROFILE_8_1\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dolby-vision-profile-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DolbyVisionProfile
---
