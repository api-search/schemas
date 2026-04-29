---
description: Settings related to SRT captions. SRT is a sidecar format that holds captions in a file that is separate from the video container. Set up sidecar captions in the same output group, but different output from your video. When you work directly in your JSON job specification, include this object and any required children when you set destinationType to SRT.
layout: schema
name: SrtDestinationSettings
properties_list:
- description: ''
  name: StylePassthrough
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-srt-destination-settings-schema.json
slug: mediaconvert-api-srt-destination-settings
source_filename: mediaconvert-api-srt-destination-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-srt-destination-settings-schema.json\",\n  \"title\": \"SrtDestinationSettings\",\n  \"description\": \"Settings related to SRT captions. SRT is a sidecar format that holds captions in a file that is separate from the video container. Set up sidecar captions in the same output group, but different output from your video. When you work directly in your JSON job specification, include this object and any required children when you set destinationType to SRT.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StylePassthrough\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SrtStylePassthrough\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"stylePassthrough\"\n          },\n          \"description\": \"Set Style passthrough (StylePassthrough)\
  \ to ENABLED to use the available style, color, and position information from your input captions. MediaConvert uses default settings for any missing style and position information in your input captions. Set Style passthrough to DISABLED, or leave blank, to ignore the style and position information from your input captions and use simplified output captions.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-srt-destination-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: SrtDestinationSettings
---
