---
description: 'To include key-length-value metadata in this output: Set KLV metadata insertion to Passthrough. MediaConvert reads KLV metadata present in your input and writes each instance to a separate event message box in the output, according to MISB ST1910.1. To exclude this KLV metadata: Set KLV metadata insertion to None or leave blank.'
layout: schema
name: MpdKlvMetadata
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-mpd-klv-metadata-schema.json
slug: mediaconvert-api-mpd-klv-metadata
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mpd-klv-metadata-schema.json\",\n  \"title\": \"MpdKlvMetadata\",\n  \"description\": \"To include key-length-value metadata in this output: Set KLV metadata insertion to Passthrough. MediaConvert reads KLV metadata present in your input and writes each instance to a separate event message box in the output, according to MISB ST1910.1. To exclude this KLV metadata: Set KLV metadata insertion to None or leave blank.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"NONE\",\n    \"PASSTHROUGH\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mpd-klv-metadata-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: MpdKlvMetadata
---
