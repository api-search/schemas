---
description: A preset is a collection of preconfigured media conversion settings that you want MediaConvert to apply to the output during the conversion process.
layout: schema
name: Preset
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: Category
  type: object
- description: ''
  name: CreatedAt
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: LastUpdated
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Settings
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-preset-schema.json
slug: mediaconvert-api-preset
source_filename: mediaconvert-api-preset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-preset-schema.json\",\n  \"title\": \"Preset\",\n  \"description\": \"A preset is a collection of preconfigured media conversion settings that you want MediaConvert to apply to the output during the conversion process.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"An identifier for this resource that is unique within all of AWS.\"\n        }\n      ]\n    },\n    \"Category\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"category\"\n          },\n  \
  \        \"description\": \"An optional category you create to organize your presets.\"\n        }\n      ]\n    },\n    \"CreatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"createdAt\"\n          },\n          \"description\": \"The timestamp in epoch seconds for preset creation.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"An optional description you create for each preset.\"\n        }\n      ]\n    },\n    \"LastUpdated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"lastUpdated\"\n          },\n          \"description\"\
  : \"The timestamp in epoch seconds when the preset was last updated.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"A name you create for each preset. Each name must be unique within your account.\"\n        }\n      ]\n    },\n    \"Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PresetSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"settings\"\n          },\n          \"description\": \"Settings for preset\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Type\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"type\"\n          },\n          \"description\": \"A preset can be of two types: system or custom. System or\
  \ built-in preset can't be modified or deleted by the user.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Settings\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-preset-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Preset
---
