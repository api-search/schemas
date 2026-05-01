---
description: Settings related to TTML captions. TTML is a sidecar format that holds captions in a file that is separate from the video container. Set up sidecar captions in the same output group, but different output from your video. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/ttml-and-webvtt-output-captions.html. When you work directly in your JSON job specification, include this object and any required children when you set destinationType to TTML.
layout: schema
name: TtmlDestinationSettings
properties_list:
- description: ''
  name: StylePassthrough
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-ttml-destination-settings-schema.json
slug: mediaconvert-api-ttml-destination-settings
source_filename: mediaconvert-api-ttml-destination-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-ttml-destination-settings-schema.json\",\n  \"title\": \"TtmlDestinationSettings\",\n  \"description\": \"Settings related to TTML captions. TTML is a sidecar format that holds captions in a file that is separate from the video container. Set up sidecar captions in the same output group, but different output from your video. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/ttml-and-webvtt-output-captions.html. When you work directly in your JSON job specification, include this object and any required children when you set destinationType to TTML.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StylePassthrough\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TtmlStylePassthrough\"\n        },\n        {\n          \"\
  xml\": {\n            \"name\": \"stylePassthrough\"\n          },\n          \"description\": \"Pass through style and position information from a TTML-like input source (TTML, IMSC, SMPTE-TT) to the TTML output.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-ttml-destination-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: TtmlDestinationSettings
---
