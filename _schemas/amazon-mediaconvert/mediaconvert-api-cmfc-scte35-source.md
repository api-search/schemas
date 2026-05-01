---
description: Ignore this setting unless you have SCTE-35 markers in your input video file. Choose Passthrough (PASSTHROUGH) if you want SCTE-35 markers that appear in your input to also appear in this output. Choose None (NONE) if you don't want those SCTE-35 markers in this output.
layout: schema
name: CmfcScte35Source
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-cmfc-scte35-source-schema.json
slug: mediaconvert-api-cmfc-scte35-source
source_filename: mediaconvert-api-cmfc-scte35-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-cmfc-scte35-source-schema.json\",\n  \"title\": \"CmfcScte35Source\",\n  \"description\": \"Ignore this setting unless you have SCTE-35 markers in your input video file. Choose Passthrough (PASSTHROUGH) if you want SCTE-35 markers that appear in your input to also appear in this output. Choose None (NONE) if you don't want those SCTE-35 markers in this output.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"PASSTHROUGH\",\n    \"NONE\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-cmfc-scte35-source-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: CmfcScte35Source
---
