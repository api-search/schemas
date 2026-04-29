---
description: Specify the bitstream mode for the E-AC-3 stream that the encoder emits. For more information about the EAC3 bitstream mode, see ATSC A/52-2012 (Annex E).
layout: schema
name: Eac3BitstreamMode
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-eac3-bitstream-mode-schema.json
slug: mediaconvert-api-eac3-bitstream-mode
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-eac3-bitstream-mode-schema.json\",\n  \"title\": \"Eac3BitstreamMode\",\n  \"description\": \"Specify the bitstream mode for the E-AC-3 stream that the encoder emits. For more information about the EAC3 bitstream mode, see ATSC A/52-2012 (Annex E).\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"COMPLETE_MAIN\",\n    \"COMMENTARY\",\n    \"EMERGENCY\",\n    \"HEARING_IMPAIRED\",\n    \"VISUALLY_IMPAIRED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-eac3-bitstream-mode-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Eac3BitstreamMode
---
