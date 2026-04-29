---
description: Maximum CDI input resolution; SD is 480i and 576i up to 30 frames-per-second (fps), HD is 720p up to 60 fps / 1080i up to 30 fps, FHD is 1080p up to 60 fps, UHD is 2160p up to 60 fps
layout: schema
name: CdiInputResolution
properties_list: []
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-cdi-input-resolution-schema.json
slug: medialive-api-cdi-input-resolution
source_filename: medialive-api-cdi-input-resolution-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-cdi-input-resolution-schema.json\",\n  \"title\": \"CdiInputResolution\",\n  \"description\": \"Maximum CDI input resolution; SD is 480i and 576i up to 30 frames-per-second (fps), HD is 720p up to 60 fps / 1080i up to 30 fps, FHD is 1080p up to 60 fps, UHD is 2160p up to 60 fps\\n\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"SD\",\n    \"HD\",\n    \"FHD\",\n    \"UHD\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-cdi-input-resolution-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CdiInputResolution
---
