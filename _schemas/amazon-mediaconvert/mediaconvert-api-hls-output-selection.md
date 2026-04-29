---
description: Indicates whether the .m3u8 manifest file should be generated for this HLS output group.
layout: schema
name: HlsOutputSelection
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-hls-output-selection-schema.json
slug: mediaconvert-api-hls-output-selection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-output-selection-schema.json\",\n  \"title\": \"HlsOutputSelection\",\n  \"description\": \"Indicates whether the .m3u8 manifest file should be generated for this HLS output group.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"MANIFESTS_AND_SEGMENTS\",\n    \"SEGMENTS_ONLY\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-output-selection-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: HlsOutputSelection
---
