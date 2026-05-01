---
description: Settings for a noise reducer filter
layout: schema
name: NoiseReducerFilterSettings
properties_list:
- description: ''
  name: Strength
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-noise-reducer-filter-settings-schema.json
slug: mediaconvert-api-noise-reducer-filter-settings
source_filename: mediaconvert-api-noise-reducer-filter-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-noise-reducer-filter-settings-schema.json\",\n  \"title\": \"NoiseReducerFilterSettings\",\n  \"description\": \"Settings for a noise reducer filter\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Strength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max3\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"strength\"\n          },\n          \"description\": \"Relative strength of noise reducing filter. Higher values produce stronger filtering.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-noise-reducer-filter-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: NoiseReducerFilterSettings
---
