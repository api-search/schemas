---
description: Settings for F4v container
layout: schema
name: F4vSettings
properties_list:
- description: ''
  name: MoovPlacement
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-f4v-settings-schema.json
slug: mediaconvert-api-f4v-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-f4v-settings-schema.json\",\n  \"title\": \"F4vSettings\",\n  \"description\": \"Settings for F4v container\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MoovPlacement\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/F4vMoovPlacement\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"moovPlacement\"\n          },\n          \"description\": \"If set to PROGRESSIVE_DOWNLOAD, the MOOV atom is relocated to the beginning of the archive as required for progressive downloading. Otherwise it is placed normally at the end.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-f4v-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: F4vSettings
---
