---
description: UpdatePresetRequest schema from Amazon MediaConvert API
layout: schema
name: UpdatePresetRequest
properties_list:
- description: ''
  name: Category
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Settings
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-update-preset-request-schema.json
slug: mediaconvert-api-update-preset-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-update-preset-request-schema.json\",\n  \"title\": \"UpdatePresetRequest\",\n  \"description\": \"UpdatePresetRequest schema from Amazon MediaConvert API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Category\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"category\"\n          },\n          \"description\": \"The new category for the preset, if you are changing it.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"The new description for the preset,\
  \ if you are changing it.\"\n        }\n      ]\n    },\n    \"Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PresetSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"settings\"\n          },\n          \"description\": \"Settings for preset\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-update-preset-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UpdatePresetRequest
---
