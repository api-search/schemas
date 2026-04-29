---
description: CreatePresetRequest schema from Amazon MediaConvert API
layout: schema
name: CreatePresetRequest
properties_list:
- description: ''
  name: Category
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Settings
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-create-preset-request-schema.json
slug: mediaconvert-api-create-preset-request
source_filename: mediaconvert-api-create-preset-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-create-preset-request-schema.json\",\n  \"title\": \"CreatePresetRequest\",\n  \"description\": \"CreatePresetRequest schema from Amazon MediaConvert API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Category\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"category\"\n          },\n          \"description\": \"Optional. A category for the preset you are creating.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"Optional. A description of the preset\
  \ you are creating.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the preset you are creating.\"\n        }\n      ]\n    },\n    \"Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PresetSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"settings\"\n          },\n          \"description\": \"Settings for preset\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"The tags that you want to add to the resource. You can tag resources with a key-value pair or with only a key.\"\n        }\n      ]\n \
  \   }\n  },\n  \"required\": [\n    \"Settings\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-create-preset-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CreatePresetRequest
---
