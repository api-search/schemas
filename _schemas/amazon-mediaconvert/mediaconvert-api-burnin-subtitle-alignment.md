---
description: Specify the alignment of your captions. If no explicit x_position is provided, setting alignment to centered will placethe captions at the bottom center of the output. Similarly, setting a left alignment willalign captions to the bottom left of the output. If x and y positions are given in conjunction with the alignment parameter, the font will be justified (either left or centered) relative to those coordinates.
layout: schema
name: BurninSubtitleAlignment
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-burnin-subtitle-alignment-schema.json
slug: mediaconvert-api-burnin-subtitle-alignment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-burnin-subtitle-alignment-schema.json\",\n  \"title\": \"BurninSubtitleAlignment\",\n  \"description\": \"Specify the alignment of your captions. If no explicit x_position is provided, setting alignment to centered will placethe captions at the bottom center of the output. Similarly, setting a left alignment willalign captions to the bottom left of the output. If x and y positions are given in conjunction with the alignment parameter, the font will be justified (either left or centered) relative to those coordinates.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"CENTERED\",\n    \"LEFT\",\n    \"AUTO\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-burnin-subtitle-alignment-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: BurninSubtitleAlignment
---
