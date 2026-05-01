---
description: H264 Color Space Settings
layout: schema
name: H264ColorSpaceSettings
properties_list:
- description: ''
  name: ColorSpacePassthroughSettings
  type: object
- description: ''
  name: Rec601Settings
  type: object
- description: ''
  name: Rec709Settings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-h264-color-space-settings-schema.json
slug: medialive-api-h264-color-space-settings
source_filename: medialive-api-h264-color-space-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-h264-color-space-settings-schema.json\",\n  \"title\": \"H264ColorSpaceSettings\",\n  \"description\": \"H264 Color Space Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ColorSpacePassthroughSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ColorSpacePassthroughSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"colorSpacePassthroughSettings\"\n          }\n        }\n      ]\n    },\n    \"Rec601Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Rec601Settings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"rec601Settings\"\n          }\n        }\n      ]\n    },\n    \"Rec709Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\":\
  \ \"#/components/schemas/Rec709Settings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"rec709Settings\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-h264-color-space-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: H264ColorSpaceSettings
---
