---
description: Group of outputs
layout: schema
name: OutputGroup
properties_list:
- description: ''
  name: AutomatedEncodingSettings
  type: object
- description: ''
  name: CustomName
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: OutputGroupSettings
  type: object
- description: ''
  name: Outputs
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-output-group-schema.json
slug: mediaconvert-api-output-group
source_filename: mediaconvert-api-output-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-output-group-schema.json\",\n  \"title\": \"OutputGroup\",\n  \"description\": \"Group of outputs\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutomatedEncodingSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutomatedEncodingSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"automatedEncodingSettings\"\n          },\n          \"description\": \"Use automated encoding to have MediaConvert choose your encoding settings for you, based on characteristics of your input video.\"\n        }\n      ]\n    },\n    \"CustomName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"customName\"\n         \
  \ },\n          \"description\": \"Use Custom Group Name (CustomName) to specify a name for the output group. This value is displayed on the console and can make your job settings JSON more human-readable. It does not affect your outputs. Use up to twelve characters that are either letters, numbers, spaces, or underscores.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"Name of the output group\"\n        }\n      ]\n    },\n    \"OutputGroupSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputGroupSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outputGroupSettings\"\n          },\n          \"description\": \"Output Group settings, including type\"\n        }\n      ]\n    },\n    \"Outputs\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/__listOfOutput\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outputs\"\n          },\n          \"description\": \"This object holds groups of encoding settings, one group of settings per output.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-output-group-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: OutputGroup
---
