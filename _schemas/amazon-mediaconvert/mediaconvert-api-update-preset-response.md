---
description: UpdatePresetResponse schema from Amazon MediaConvert API
layout: schema
name: UpdatePresetResponse
properties_list:
- description: ''
  name: Preset
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-update-preset-response-schema.json
slug: mediaconvert-api-update-preset-response
source_filename: mediaconvert-api-update-preset-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-update-preset-response-schema.json\",\n  \"title\": \"UpdatePresetResponse\",\n  \"description\": \"UpdatePresetResponse schema from Amazon MediaConvert API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Preset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Preset\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"preset\"\n          },\n          \"description\": \"A preset is a collection of preconfigured media conversion settings that you want MediaConvert to apply to the output during the conversion process.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-update-preset-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UpdatePresetResponse
---
