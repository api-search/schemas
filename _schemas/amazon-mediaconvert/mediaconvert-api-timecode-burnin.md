---
description: Settings for burning the output timecode and specified prefix into the output.
layout: schema
name: TimecodeBurnin
properties_list:
- description: ''
  name: FontSize
  type: object
- description: ''
  name: Position
  type: object
- description: ''
  name: Prefix
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-timecode-burnin-schema.json
slug: mediaconvert-api-timecode-burnin
source_filename: mediaconvert-api-timecode-burnin-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-timecode-burnin-schema.json\",\n  \"title\": \"TimecodeBurnin\",\n  \"description\": \"Settings for burning the output timecode and specified prefix into the output.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FontSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin10Max48\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fontSize\"\n          },\n          \"description\": \"Use Font Size (FontSize) to set the font size of any burned-in timecode. Valid values are 10, 16, 32, 48.\"\n        }\n      ]\n    },\n    \"Position\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimecodeBurninPosition\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"position\"\
  \n          },\n          \"description\": \"Use Position (Position) under under Timecode burn-in (TimecodeBurnIn) to specify the location the burned-in timecode on output video.\"\n        }\n      ]\n    },\n    \"Prefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPattern\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"prefix\"\n          },\n          \"description\": \"Use Prefix (Prefix) to place ASCII characters before any burned-in timecode. For example, a prefix of \\\"EZ-\\\" will result in the timecode \\\"EZ-00:00:00:00\\\". Provide either the characters themselves or the ASCII code equivalents. The supported range of characters is 0x20 through 0x7e. This includes letters, numbers, and all special characters represented on a standard English keyboard.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-timecode-burnin-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: TimecodeBurnin
---
