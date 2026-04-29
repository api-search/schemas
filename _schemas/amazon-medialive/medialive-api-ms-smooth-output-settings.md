---
description: Ms Smooth Output Settings
layout: schema
name: MsSmoothOutputSettings
properties_list:
- description: ''
  name: H265PackagingType
  type: object
- description: ''
  name: NameModifier
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-ms-smooth-output-settings-schema.json
slug: medialive-api-ms-smooth-output-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-ms-smooth-output-settings-schema.json\",\n  \"title\": \"MsSmoothOutputSettings\",\n  \"description\": \"Ms Smooth Output Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"H265PackagingType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MsSmoothH265PackagingType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"h265PackagingType\"\n          },\n          \"description\": \"Only applicable when this output is referencing an H.265 video description.\\nSpecifies whether MP4 segments should be packaged as HEV1 or HVC1.\"\n        }\n      ]\n    },\n    \"NameModifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\"\
  : \"nameModifier\"\n          },\n          \"description\": \"String concatenated to the end of the destination filename.  Required for multiple outputs of the same type.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-ms-smooth-output-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: MsSmoothOutputSettings
---
