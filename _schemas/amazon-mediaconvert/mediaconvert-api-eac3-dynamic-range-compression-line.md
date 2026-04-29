---
description: 'Choose the Dolby Digital dynamic range control (DRC) profile that MediaConvert uses when encoding the metadata in the Dolby Digital stream for the line operating mode. Related setting: When you use this setting, MediaConvert ignores any value you provide for Dynamic range compression profile (DynamicRangeCompressionProfile). For information about the Dolby Digital DRC operating modes and profiles, see the Dynamic Range Control chapter of the Dolby Metadata Guide at https://developer.dolby.com/globalassets/professional/documents/dolby-metadata-guide.pdf.'
layout: schema
name: Eac3DynamicRangeCompressionLine
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-eac3-dynamic-range-compression-line-schema.json
slug: mediaconvert-api-eac3-dynamic-range-compression-line
source_filename: mediaconvert-api-eac3-dynamic-range-compression-line-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-eac3-dynamic-range-compression-line-schema.json\",\n  \"title\": \"Eac3DynamicRangeCompressionLine\",\n  \"description\": \"Choose the Dolby Digital dynamic range control (DRC) profile that MediaConvert uses when encoding the metadata in the Dolby Digital stream for the line operating mode. Related setting: When you use this setting, MediaConvert ignores any value you provide for Dynamic range compression profile (DynamicRangeCompressionProfile). For information about the Dolby Digital DRC operating modes and profiles, see the Dynamic Range Control chapter of the Dolby Metadata Guide at https://developer.dolby.com/globalassets/professional/documents/dolby-metadata-guide.pdf.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"NONE\",\n    \"FILM_STANDARD\",\n    \"FILM_LIGHT\",\n   \
  \ \"MUSIC_STANDARD\",\n    \"MUSIC_LIGHT\",\n    \"SPEECH\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-eac3-dynamic-range-compression-line-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Eac3DynamicRangeCompressionLine
---
