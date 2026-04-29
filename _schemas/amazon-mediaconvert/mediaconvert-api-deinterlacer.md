---
description: Settings for deinterlacer
layout: schema
name: Deinterlacer
properties_list:
- description: ''
  name: Algorithm
  type: object
- description: ''
  name: Control
  type: object
- description: ''
  name: Mode
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-deinterlacer-schema.json
slug: mediaconvert-api-deinterlacer
source_filename: mediaconvert-api-deinterlacer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-deinterlacer-schema.json\",\n  \"title\": \"Deinterlacer\",\n  \"description\": \"Settings for deinterlacer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Algorithm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeinterlaceAlgorithm\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"algorithm\"\n          },\n          \"description\": \"Only applies when you set Deinterlacer (DeinterlaceMode) to Deinterlace (DEINTERLACE) or Adaptive (ADAPTIVE). Motion adaptive interpolate (INTERPOLATE) produces sharper pictures, while blend (BLEND) produces smoother motion. Use (INTERPOLATE_TICKER) OR (BLEND_TICKER) if your source file includes a ticker, such as a scrolling headline at the bottom of the frame.\"\n        }\n      ]\n \
  \   },\n    \"Control\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeinterlacerControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"control\"\n          },\n          \"description\": \"- When set to NORMAL (default), the deinterlacer does not convert frames that are tagged in metadata as progressive. It will only convert those that are tagged as some other type. - When set to FORCE_ALL_FRAMES, the deinterlacer converts every frame to progressive - even those that are already tagged as progressive. Turn Force mode on only if there is a good chance that the metadata has tagged frames as progressive when they are not progressive. Do not turn on otherwise; processing frames that are already progressive into progressive will probably result in lower quality video.\"\n        }\n      ]\n    },\n    \"Mode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeinterlacerMode\"\n        },\n        {\n \
  \         \"xml\": {\n            \"name\": \"mode\"\n          },\n          \"description\": \"Use Deinterlacer (DeinterlaceMode) to choose how the service will do deinterlacing. Default is Deinterlace. - Deinterlace converts interlaced to progressive. - Inverse telecine converts Hard Telecine 29.97i to progressive 23.976p. - Adaptive auto-detects and converts to progressive.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-deinterlacer-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Deinterlacer
---
