---
description: CreatePresetResponse schema from Amazon MediaConvert API
layout: schema
name: CreatePresetResponse
properties_list:
- description: ''
  name: Preset
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-create-preset-response-schema.json
slug: mediaconvert-api-create-preset-response
source_filename: mediaconvert-api-create-preset-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-create-preset-response-schema.json\",\n  \"title\": \"CreatePresetResponse\",\n  \"description\": \"CreatePresetResponse schema from Amazon MediaConvert API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Preset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Preset\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"preset\"\n          },\n          \"description\": \"A preset is a collection of preconfigured media conversion settings that you want MediaConvert to apply to the output during the conversion process.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-create-preset-response-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: CreatePresetResponse
---
