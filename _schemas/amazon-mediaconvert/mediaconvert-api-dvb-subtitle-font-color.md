---
description: Specify the color of the captions text. Leave Font color (FontColor) blank and set Style passthrough (StylePassthrough) to enabled to use the font color data from your input captions, if present. Within your job settings, all of your DVB-Sub settings must be identical.
layout: schema
name: DvbSubtitleFontColor
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-dvb-subtitle-font-color-schema.json
slug: mediaconvert-api-dvb-subtitle-font-color
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dvb-subtitle-font-color-schema.json\",\n  \"title\": \"DvbSubtitleFontColor\",\n  \"description\": \"Specify the color of the captions text. Leave Font color (FontColor) blank and set Style passthrough (StylePassthrough) to enabled to use the font color data from your input captions, if present. Within your job settings, all of your DVB-Sub settings must be identical.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"WHITE\",\n    \"BLACK\",\n    \"YELLOW\",\n    \"RED\",\n    \"GREEN\",\n    \"BLUE\",\n    \"HEX\",\n    \"AUTO\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dvb-subtitle-font-color-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DvbSubtitleFontColor
---
