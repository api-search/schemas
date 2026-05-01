---
description: Type of output group (File group, Apple HLS, DASH ISO, Microsoft Smooth Streaming, CMAF)
layout: schema
name: OutputGroupType
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-output-group-type-schema.json
slug: mediaconvert-api-output-group-type
source_filename: mediaconvert-api-output-group-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-output-group-type-schema.json\",\n  \"title\": \"OutputGroupType\",\n  \"description\": \"Type of output group (File group, Apple HLS, DASH ISO, Microsoft Smooth Streaming, CMAF)\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"HLS_GROUP_SETTINGS\",\n    \"DASH_ISO_GROUP_SETTINGS\",\n    \"FILE_GROUP_SETTINGS\",\n    \"MS_SMOOTH_GROUP_SETTINGS\",\n    \"CMAF_GROUP_SETTINGS\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-output-group-type-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: OutputGroupType
---
