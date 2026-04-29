---
description: Specify the color of the shadow cast by the captions. Leave Shadow color (ShadowColor) blank and set Style passthrough (StylePassthrough) to enabled to use the shadow color data from your input captions, if present. Within your job settings, all of your DVB-Sub settings must be identical.
layout: schema
name: DvbSubtitleShadowColor
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-dvb-subtitle-shadow-color-schema.json
slug: mediaconvert-api-dvb-subtitle-shadow-color
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dvb-subtitle-shadow-color-schema.json\",\n  \"title\": \"DvbSubtitleShadowColor\",\n  \"description\": \"Specify the color of the shadow cast by the captions. Leave Shadow color (ShadowColor) blank and set Style passthrough (StylePassthrough) to enabled to use the shadow color data from your input captions, if present. Within your job settings, all of your DVB-Sub settings must be identical.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"NONE\",\n    \"BLACK\",\n    \"WHITE\",\n    \"AUTO\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dvb-subtitle-shadow-color-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DvbSubtitleShadowColor
---
