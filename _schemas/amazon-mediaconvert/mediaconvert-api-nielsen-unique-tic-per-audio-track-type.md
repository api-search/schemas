---
description: To create assets that have the same TIC values in each audio track, keep the default value Share TICs (SAME_TICS_PER_TRACK). To create assets that have unique TIC values for each audio track, choose Use unique TICs (RESERVE_UNIQUE_TICS_PER_TRACK).
layout: schema
name: NielsenUniqueTicPerAudioTrackType
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-nielsen-unique-tic-per-audio-track-type-schema.json
slug: mediaconvert-api-nielsen-unique-tic-per-audio-track-type
source_filename: mediaconvert-api-nielsen-unique-tic-per-audio-track-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-nielsen-unique-tic-per-audio-track-type-schema.json\",\n  \"title\": \"NielsenUniqueTicPerAudioTrackType\",\n  \"description\": \"To create assets that have the same TIC values in each audio track, keep the default value Share TICs (SAME_TICS_PER_TRACK). To create assets that have unique TIC values for each audio track, choose Use unique TICs (RESERVE_UNIQUE_TICS_PER_TRACK).\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"RESERVE_UNIQUE_TICS_PER_TRACK\",\n    \"SAME_TICS_PER_TRACK\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-nielsen-unique-tic-per-audio-track-type-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: NielsenUniqueTicPerAudioTrackType
---
