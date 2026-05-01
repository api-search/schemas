---
description: The video encoding method for your MPEG-4 AVC output. Keep the default value, PAFF, to have MediaConvert use PAFF encoding for interlaced outputs. Choose Force field (FORCE_FIELD) to disable PAFF encoding and create separate interlaced fields. Choose MBAFF to disable PAFF and have MediaConvert use MBAFF encoding for interlaced outputs.
layout: schema
name: H264FieldEncoding
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-h264-field-encoding-schema.json
slug: mediaconvert-api-h264-field-encoding
source_filename: mediaconvert-api-h264-field-encoding-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-h264-field-encoding-schema.json\",\n  \"title\": \"H264FieldEncoding\",\n  \"description\": \"The video encoding method for your MPEG-4 AVC output. Keep the default value, PAFF, to have MediaConvert use PAFF encoding for interlaced outputs. Choose Force field (FORCE_FIELD) to disable PAFF encoding and create separate interlaced fields. Choose MBAFF to disable PAFF and have MediaConvert use MBAFF encoding for interlaced outputs.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"PAFF\",\n    \"FORCE_FIELD\",\n    \"MBAFF\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-h264-field-encoding-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: H264FieldEncoding
---
