---
description: 'Unless you need Omneon compatibility: Keep the default value, None. To make this output compatible with Omneon: Choose Omneon. When you do, MediaConvert increases the length of the ''elst'' edit list atom. Note that this might cause file rejections when a recipient of the output file doesn''t expect this extra padding.'
layout: schema
name: MovPaddingControl
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-mov-padding-control-schema.json
slug: mediaconvert-api-mov-padding-control
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mov-padding-control-schema.json\",\n  \"title\": \"MovPaddingControl\",\n  \"description\": \"Unless you need Omneon compatibility: Keep the default value, None. To make this output compatible with Omneon: Choose Omneon. When you do, MediaConvert increases the length of the 'elst' edit list atom. Note that this might cause file rejections when a recipient of the output file doesn't expect this extra padding.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"OMNEON\",\n    \"NONE\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mov-padding-control-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: MovPaddingControl
---
