---
description: Timecode Burnin Settings
layout: schema
name: TimecodeBurninSettings
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
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-timecode-burnin-settings-schema.json
slug: medialive-api-timecode-burnin-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-timecode-burnin-settings-schema.json\",\n  \"title\": \"TimecodeBurninSettings\",\n  \"description\": \"Timecode Burnin Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FontSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimecodeBurninFontSize\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fontSize\"\n          },\n          \"description\": \"Choose a timecode burn-in font size\"\n        }\n      ]\n    },\n    \"Position\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimecodeBurninPosition\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"position\"\n          },\n          \"description\": \"Choose a timecode burn-in output position\"\n        }\n     \
  \ ]\n    },\n    \"Prefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMax255\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"prefix\"\n          },\n          \"description\": \"Create a timecode burn-in prefix (optional)\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Position\",\n    \"FontSize\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-timecode-burnin-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: TimecodeBurninSettings
---
