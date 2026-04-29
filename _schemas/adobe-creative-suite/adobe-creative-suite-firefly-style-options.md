---
description: Style guidance for image generation
layout: schema
name: StyleOptions
properties_list:
- description: List of style preset identifiers to apply
  name: presets
  type: array
- description: Style influence strength from 1 (subtle) to 100 (strong)
  name: strength
  type: integer
- description: ''
  name: referenceImage
  type: object
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-firefly-style-options-schema.json
slug: adobe-creative-suite-firefly-style-options
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-firefly-style-options-schema.json\",\n  \"title\": \"StyleOptions\",\n  \"description\": \"Style guidance for image generation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"presets\": {\n      \"type\": \"array\",\n      \"description\": \"List of style preset identifiers to apply\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"photo\",\n          \"art\",\n          \"graphic\",\n          \"bw\",\n          \"cool_colors\",\n          \"warm_tone\",\n          \"muted_color\",\n          \"vibrant_color\",\n          \"pastel_color\",\n          \"golden_hour\",\n          \"closeup_portrait\",\n          \"wide_angle\",\n          \"aerial_view\",\n          \"landscape_photography\"\n        ]\n      },\n      \"example\":\
  \ [\n        \"photo\",\n        \"golden_hour\"\n      ]\n    },\n    \"strength\": {\n      \"type\": \"integer\",\n      \"description\": \"Style influence strength from 1 (subtle) to 100 (strong)\",\n      \"minimum\": 1,\n      \"maximum\": 100,\n      \"example\": 60\n    },\n    \"referenceImage\": {\n      \"$ref\": \"#/components/schemas/InputImageReference\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-firefly-style-options-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: StyleOptions
---
