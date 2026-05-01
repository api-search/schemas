---
description: Specify whether the encoder uses B-frames as reference frames for other pictures in the same GOP. Choose Allow (ENABLED) to allow the encoder to use B-frames as reference frames. Choose Don't allow (DISABLED) to prevent the encoder from using B-frames as reference frames.
layout: schema
name: XavcGopBReference
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-xavc-gop-b-reference-schema.json
slug: mediaconvert-api-xavc-gop-b-reference
source_filename: mediaconvert-api-xavc-gop-b-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-xavc-gop-b-reference-schema.json\",\n  \"title\": \"XavcGopBReference\",\n  \"description\": \"Specify whether the encoder uses B-frames as reference frames for other pictures in the same GOP. Choose Allow (ENABLED) to allow the encoder to use B-frames as reference frames. Choose Don't allow (DISABLED) to prevent the encoder from using B-frames as reference frames.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"DISABLED\",\n    \"ENABLED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-xavc-gop-b-reference-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: XavcGopBReference
---
