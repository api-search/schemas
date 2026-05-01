---
description: 'Specify the type of the ID3 frame (timedMetadataId3Frame) to use for ID3 timestamps (timedMetadataId3Period) in your output. To include ID3 timestamps: Specify PRIV (PRIV) or TDRL (TDRL) and set ID3 metadata (timedMetadata) to Passthrough (PASSTHROUGH). To exclude ID3 timestamps: Set ID3 timestamp frame type to None (NONE).'
layout: schema
name: HlsTimedMetadataId3Frame
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-hls-timed-metadata-id3-frame-schema.json
slug: mediaconvert-api-hls-timed-metadata-id3-frame
source_filename: mediaconvert-api-hls-timed-metadata-id3-frame-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-timed-metadata-id3-frame-schema.json\",\n  \"title\": \"HlsTimedMetadataId3Frame\",\n  \"description\": \"Specify the type of the ID3 frame (timedMetadataId3Frame) to use for ID3 timestamps (timedMetadataId3Period) in your output. To include ID3 timestamps: Specify PRIV (PRIV) or TDRL (TDRL) and set ID3 metadata (timedMetadata) to Passthrough (PASSTHROUGH). To exclude ID3 timestamps: Set ID3 timestamp frame type to None (NONE).\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"NONE\",\n    \"PRIV\",\n    \"TDRL\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-timed-metadata-id3-frame-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: HlsTimedMetadataId3Frame
---
