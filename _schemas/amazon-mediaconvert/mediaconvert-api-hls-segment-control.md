---
description: 'When set to SINGLE_FILE, emits program as a single media resource (.ts) file, uses #EXT-X-BYTERANGE tags to index segment for playback.'
layout: schema
name: HlsSegmentControl
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-hls-segment-control-schema.json
slug: mediaconvert-api-hls-segment-control
source_filename: mediaconvert-api-hls-segment-control-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-segment-control-schema.json\",\n  \"title\": \"HlsSegmentControl\",\n  \"description\": \"When set to SINGLE_FILE, emits program as a single media resource (.ts) file, uses #EXT-X-BYTERANGE tags to index segment for playback.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"SINGLE_FILE\",\n    \"SEGMENTED_FILES\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-segment-control-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: HlsSegmentControl
---
