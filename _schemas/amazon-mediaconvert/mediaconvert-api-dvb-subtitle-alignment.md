---
description: Specify the alignment of your captions. If no explicit x_position is provided, setting alignment to centered will placethe captions at the bottom center of the output. Similarly, setting a left alignment willalign captions to the bottom left of the output. If x and y positions are given in conjunction with the alignment parameter, the font will be justified (either left or centered) relative to those coordinates. Within your job settings, all of your DVB-Sub settings must be identical.
layout: schema
name: DvbSubtitleAlignment
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-dvb-subtitle-alignment-schema.json
slug: mediaconvert-api-dvb-subtitle-alignment
source_filename: mediaconvert-api-dvb-subtitle-alignment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dvb-subtitle-alignment-schema.json\",\n  \"title\": \"DvbSubtitleAlignment\",\n  \"description\": \"Specify the alignment of your captions. If no explicit x_position is provided, setting alignment to centered will placethe captions at the bottom center of the output. Similarly, setting a left alignment willalign captions to the bottom left of the output. If x and y positions are given in conjunction with the alignment parameter, the font will be justified (either left or centered) relative to those coordinates. Within your job settings, all of your DVB-Sub settings must be identical.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"CENTERED\",\n    \"LEFT\",\n    \"AUTO\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dvb-subtitle-alignment-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: DvbSubtitleAlignment
---
