---
description: Selects method of inserting SDT information into output stream. "Follow input SDT" copies SDT information from input stream to output stream. "Follow input SDT if present" copies SDT information from input stream to output stream if SDT information is present in the input, otherwise it will fall back on the user-defined values. Enter "SDT Manually" means user will enter the SDT information. "No SDT" means output stream will not contain SDT information.
layout: schema
name: OutputSdt
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-output-sdt-schema.json
slug: mediaconvert-api-output-sdt
source_filename: mediaconvert-api-output-sdt-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-output-sdt-schema.json\",\n  \"title\": \"OutputSdt\",\n  \"description\": \"Selects method of inserting SDT information into output stream. \\\"Follow input SDT\\\" copies SDT information from input stream to output stream. \\\"Follow input SDT if present\\\" copies SDT information from input stream to output stream if SDT information is present in the input, otherwise it will fall back on the user-defined values. Enter \\\"SDT Manually\\\" means user will enter the SDT information. \\\"No SDT\\\" means output stream will not contain SDT information.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"SDT_FOLLOW\",\n    \"SDT_FOLLOW_IF_PRESENT\",\n    \"SDT_MANUAL\",\n    \"SDT_NONE\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-output-sdt-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: OutputSdt
---
