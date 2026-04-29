---
description: ListPresetsResponse schema from Amazon MediaConvert API
layout: schema
name: ListPresetsResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: Presets
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-list-presets-response-schema.json
slug: mediaconvert-api-list-presets-response
source_filename: mediaconvert-api-list-presets-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-list-presets-response-schema.json\",\n  \"title\": \"ListPresetsResponse\",\n  \"description\": \"ListPresetsResponse schema from Amazon MediaConvert API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"Use this string to request the next batch of presets.\"\n        }\n      ]\n    },\n    \"Presets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfPreset\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"presets\"\n          },\n          \"description\": \"List of presets\"\n        }\n    \
  \  ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-list-presets-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListPresetsResponse
---
