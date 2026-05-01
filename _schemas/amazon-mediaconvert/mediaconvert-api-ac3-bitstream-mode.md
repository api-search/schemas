---
description: Specify the bitstream mode for the AC-3 stream that the encoder emits. For more information about the AC3 bitstream mode, see ATSC A/52-2012 (Annex E).
layout: schema
name: Ac3BitstreamMode
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-ac3-bitstream-mode-schema.json
slug: mediaconvert-api-ac3-bitstream-mode
source_filename: mediaconvert-api-ac3-bitstream-mode-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-ac3-bitstream-mode-schema.json\",\n  \"title\": \"Ac3BitstreamMode\",\n  \"description\": \"Specify the bitstream mode for the AC-3 stream that the encoder emits. For more information about the AC3 bitstream mode, see ATSC A/52-2012 (Annex E).\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"COMPLETE_MAIN\",\n    \"COMMENTARY\",\n    \"DIALOGUE\",\n    \"EMERGENCY\",\n    \"HEARING_IMPAIRED\",\n    \"MUSIC_AND_EFFECTS\",\n    \"VISUALLY_IMPAIRED\",\n    \"VOICE_OVER\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-ac3-bitstream-mode-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Ac3BitstreamMode
---
