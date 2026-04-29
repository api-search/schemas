---
description: 'The Coding mode that you specify determines the number of audio channels and the audio channel layout metadata in your AAC output. Valid coding modes depend on the Rate control mode and Profile that you select. The following list shows the number of audio channels and channel layout for each coding mode. * 1.0 Audio Description (Receiver Mix): One channel, C. Includes audio description data from your stereo input. For more information see ETSI TS 101 154 Annex E. * 1.0 Mono: One channel, C. * 2.0 Stereo: Two channels, L, R. * 5.1 Surround: Five channels, C, L, R, Ls, Rs, LFE.'
layout: schema
name: AacCodingMode
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-aac-coding-mode-schema.json
slug: mediaconvert-api-aac-coding-mode
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-aac-coding-mode-schema.json\",\n  \"title\": \"AacCodingMode\",\n  \"description\": \"The Coding mode that you specify determines the number of audio channels and the audio channel layout metadata in your AAC output. Valid coding modes depend on the Rate control mode and Profile that you select. The following list shows the number of audio channels and channel layout for each coding mode. * 1.0 Audio Description (Receiver Mix): One channel, C. Includes audio description data from your stereo input. For more information see ETSI TS 101 154 Annex E. * 1.0 Mono: One channel, C. * 2.0 Stereo: Two channels, L, R. * 5.1 Surround: Five channels, C, L, R, Ls, Rs, LFE.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"AD_RECEIVER_MIX\",\n    \"CODING_MODE_1_0\",\n    \"CODING_MODE_1_1\",\n\
  \    \"CODING_MODE_2_0\",\n    \"CODING_MODE_5_1\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-aac-coding-mode-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AacCodingMode
---
